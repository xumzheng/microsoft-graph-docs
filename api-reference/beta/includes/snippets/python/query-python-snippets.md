---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = QueryPostRequestBody()
requests_search_request1 = SearchRequest()
requestsSearchRequest1.EntityTypes([requestsSearchRequest1.EntityType(EntityType('externalitem'))
])

requestsSearchRequest1.ContentSources(['/external/connections/connectionfriendlyname', ])

requests_search_request1_query = SearchQuery()
requestsSearchRequest1Query.queryString = 'contoso product'


requestsSearchRequest1.query = requestsSearchRequest1Query
requestsSearchRequest1.from = 0

requestsSearchRequest1.size = 25

requestsSearchRequest1.Fields(['title', 'description', ])


requestsArray []= requestsSearchRequest1;
request_body.requests(requestsArray)





result = await client.search.query.post(request_body = request_body)


```