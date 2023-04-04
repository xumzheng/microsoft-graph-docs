---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = QueryPostRequestBody()
requestsSearchRequest1 = SearchRequest()
requestsSearchRequest1.setEntityTypes([requestsSearchRequest1.setEntityType(EntityType('chatmessage'))
])

requestsSearchRequest1Query = SearchQuery()
requestsSearchRequest1Query.setQueryString('contoso from:bob to:alice sent>2022-07-14')


requestsSearchRequest1.setQuery($requestsSearchRequest1Query)
requestsSearchRequest1.setFrom(0)

requestsSearchRequest1.setSize(15)

requestsSearchRequest1.setEnableTopResults(true)


requestsArray []= requestsSearchRequest1;
request_body.setRequests(requestsArray)




result = await client.search.query.post(request_body)


```