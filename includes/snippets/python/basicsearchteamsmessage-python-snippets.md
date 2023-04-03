---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = QueryPostRequestBody();
requestsSearchRequest1 = SearchRequest();
requestsSearchRequest1.setEntityTypes([requestsSearchRequest1.setEntityType(EntityType('chatmessage'));
]);

requestsSearchRequest1Query = SearchQuery();
requestsSearchRequest1Query.setQueryString('test');


requestsSearchRequest1.setQuery($requestsSearchRequest1Query);
requestsSearchRequest1.setFrom(0);

requestsSearchRequest1.setSize(25);


requestsArray []= requestsSearchRequest1;
requestBody.setRequests(requestsArray);




result = awaitclient.search().query().post(requestBody);


```