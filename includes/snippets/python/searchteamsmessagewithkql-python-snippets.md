---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = QueryPostRequestBody()
requestsSearchRequest1 = SearchRequest()
requestsSearchRequest1.EntityTypes([requestsSearchRequest1.EntityType(EntityType('chatmessage'))
])

requestsSearchRequest1Query = SearchQuery()
requestsSearchRequest1Query.queryString = 'contoso from:bob to:alice sent>2022-07-14'


requestsSearchRequest1.query = requestsSearchRequest1Query
requestsSearchRequest1.from = 0

requestsSearchRequest1.size = 15

requestsSearchRequest1.enableTopResults = true


requestsArray []= requestsSearchRequest1;
request_body.requests(requestsArray)




request_configuration = QueryRequestBuilderPostRequestConfiguration(
)


result = await client.search.query.post(request_body = request_body)


```