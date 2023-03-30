---
title: "Get topic through search"
description: "Retrieve the properties and relationships of Topic object. "
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: "governance"
author: "watermelonT" 
---

# Get Topic through search

Namespace: microsoft.graph

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
<!-- { "blockType": "ignored" } -->
```http
GET /search
```
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.

## Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and [topic](../resources/topic.md) object in the response body.

Note that the requestor needs to have an assigned Viva Topics license. Otherwise, the HTTP 403 Forbidden status code will be returned.
## Example
##### Request
Here is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/search
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-privilegedrole-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-privilegedrole-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-privilegedrole-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### Response
Here is an example of the response. Note: The response object shown here might be shortened for readability.

```http
Response
HTTP/1.1 200 Ok
```

```json
{
  "value": [
    {
      { "@type": "searchResult" },// Search Response
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
