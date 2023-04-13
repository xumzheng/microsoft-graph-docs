---
title: "Use the Microsoft Search API to search Topics"
description: "Retrieve the properties and relationships of Topic object. "
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: "governance"
author: "watermelonT" 
---

# Search Topics

Namespace: microsoft.graph

You can use the Microsoft Search API in Microsoft Graph to search Topics. Administrators can manage Topics in the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/MicrosoftSearch/bookmarks).

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve the properties and relationships of [topic](../resources/topic.md) object. 

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Topic.Read.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Not supported. |

## HTTP request
```http
POST /search
```
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.

## Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer {token}. Required. |

## Request body

### searchRequest

Specifies search parameters for a particular entity type

#### Properties

Name | Type | Required | Extension to elastic DSL(Default is No) | Description
-----|------|----------|------------|---------
`entityTypes` | Collection(microsoft.graph.entityType) | Y | Y| The type of entity to be returned in search results. Having multiple entityTypes specified implies the results will be merged and ranked accross the different types.
`contentSources` | Collection(Edm.String)  | N | N| The source of data to retrieve
`query` | microsoft.graph.searchQuery | Y | |The query object used to formulate search query
`from` | Edm.Int32 | Y || The offset for search results
`size` | Edm.Int32 | Y || The number of results requested in the response
`stored_fields` | Collection(Edm.String) | N || The fields that should be returned from each source entity in the response. If the field is not available on the given entity, it will not be returned. Most entities have default fields on therefore stored_field does not need to be specified. If the stored_field specifed is invalid, this will return an empty value in the response.
`enableTopResults`| boolean | N | Y | This parameter is specifc to Messages. Enables returning up to 3 relevance based results for email search. The rest of the results are ordered by date desc.
`sortProperties`| Collection(sortOption) | N | Y | Enables sorting on the specified sortable fields.
`aggregation`| Collection(aggsOption) | N | Y | Provides the aggregations to be returned.

### entityType

The type of entities to be returned in search results.

|Value
|----------
|`topic` 

### searchQuery

The query to be executed.

#### Properties

Name | Type | Required | Description
-----|------|----------|------------
`query_string` | microsoft.graph.searchQueryString | Y | A query that uses a query parser in order to parse its content.
`spellCheckType` | Edm.String | N | Possible values are "alteration/suggestion"


### searchQueryString

#### Properties

Name | Type | Required | Description
-----|------|----------|------------
`query`| Edm.String | Y | The query text to be executed. The parse syntax supported is KQL. See note below.

#### Design note: query syntax

The current supported syntax for query is KQL. All exchange entity types support a [subset of KQL ](https://docs.microsoft.com/en-us/office365/securitycompliance/keyword-queries-and-search-conditions). DriveItem supports the [full KQL](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference). Aligning KQL with ElasticSearch Filter syntax is a large project and will be considered for future release. Another consideration for KQL is ingrained user behavior for Outlooks where the user types in KQL in the search box.


## Response

If successful, this method returns a `200 OK` response code and [topic](../resources/topic.md) object in the response body.

Note that the requestor needs to have an assigned Viva Topics license. Otherwise, the HTTP 403 Forbidden status code will be returned.

### Response headers
 Name | Type | Description
------| ------| ---------
Instrumentation | String   | A unique identifier used for instrumentation purpose. Unless otherwise specified, it should not be used by the client.

### New Entity types

#### searchResult

Name | Type | Required | Description
-----|------|----------|------------
searchTerms | Collection(Edm.String) | Y | The search terms used on the query for returning results in this resultSets
hitsContainers | Collection(microsoft.graph.searchHitsContainer) | Y |A group of results satifying the query
suggestedQuery | Edm.String | N | The suggested spell correction
recourseQuery | Edm.String | N | The intial query sent by the user (in case Alternation is used)

##### Design note: Result grouping

Typical grouping is done by graph path to the entity collection. Beta API will only support 1 group. hitsContainers is retained as a collection to avoid making a schema breaking change for future scenarios.

#### searchHitsContainer

Name | Type | Description
-----|------|----------
hits | Collection(microsoft.graph.searchHit) | The results satifying the query
total | Edm.Int32  | The number of search results in the resultSet
moreResultsAvailable | Edm.Boolean  | Specifies if more results are available
aggregations | Collection(searchAggregation) | Returns the agregations

#### searchHit

Name | Type | Extension to elastic|Description
-----|------|----------|------------
_id  | Edm.String | N| The identifier of the item
_score  | Edm.Int32 | N| The rank of the result. In case of time order sort (default for messages) this value is the timestamp of the entity.
_sortField (Deprecated MVP3)  | Edm.String | Y | The sort order used for the client to able to deliniate in case of multiple orders. Default sort order is relevance. When a sortRequest is specified, the sortField is set to the value used for sorting. // DEPRECATE MVP3
_summary | Edm.String | Y| A caption for the result. Typically consisting of a sentence most relevant to the query keywords.
_contentSource | Edm.String | N| For multiple connections scenario for Connectors, indicates which connection the item is part of.
_source  | OpenType | N| The source item - Can be of type `microsoft.graph.message`, `microsoft.graph.event`, `microsoft.graph.driveItem`, `microsoft.graph.externalItem`, `microsoft.graph.site`, `microsoft.graph.drive`, `microsoft.graph.list`, `microsoft.graph.listitem`, `microsoft.graph.topic` 

#### searchAggregation

Name | Type | Description
-----|------|----------
displayName | Edm.String | The name of the refiner specified in the request (ex : "Refine by File type")
field | Edm.String | The field used to compute the agregation (ex : "FileType")
buckets | Collection(searchHitsBucket) | the buckets computed


#### searchHitsBucket

Name | Type | Description
-----|------|----------
key | Edm.String | The value of bucket (Ex : "docx")
Count | Edm.Int32 | The number of matches found for the given bucket
refinementToken | Edm.String | A token containing the encoded filter to be returned to execute the filtered query

## Example
### Request
Here is an example of the request.

# [HTTP](#tab/http)
```msgraph-interactive
POST https://graph.microsoft.com/beta/search
```

Simplest query case
Query for topics from knowledge based accessible by current person conducting the search, to retrieve topic result and to return a set of fields with this result.

```http
POST https://graph.microsoft.com/beta/search
Content-Type: application/json
Authorization: Bearer AAD_TOKEN
```

```json
{
  "requests": [{
      "entityType": "topic",
      "query": {
        "query_string": {
          "query": "topics"
        }
      }
    }
  ]
}
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../../../includes/snippets/csharp/topicsearch-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../../../includes/snippets/javascript/topicsearch-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../../../includes/snippets/java/topicsearch-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../../../includes/snippets/go/topicsearch-post-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../../../includes/snippets/powershell/topicsearch-post-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../../../includes/snippets/php/topicsearch-post-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response
Here is an example of the response. Note: The response object shown here might be shortened for readability. You can find the full list of Topics properties in [topic](../resources/topic.md) page.

```http
Response
HTTP/1.1 200 Ok
```

```json
{
  "value": [
    {
      { "@type": "searchResult" },
      "searchTerms": [
        "topics"
      ],
      "hitsContainers": [
        {
          { "@type": "searchHitsContainer" },
          "hits": [
            {
              { "@type": "searchHit" },
              "_id": ,
              "_score": 1,
              "_summary": "summary text",              
              "_source": {
                "@odata.type": "#microsoft.graph.topic",
                "primaryName": ,
                "alternateNames": ,
              }
            },
            {
            }
          ],
          "total": 5,
          "moreResultsAvailable": true
        },
        {

        }
      ]
    }
  ]
}
```
