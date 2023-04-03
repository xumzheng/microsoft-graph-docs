---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = QueryPostRequestBody();
requestsSearchRequest1 = SearchRequest();
requestsSearchRequest1.setEntityTypes([requestsSearchRequest1.setEntityType(EntityType('externalitem'));
]);

requestsSearchRequest1.setContentSources(['/external/connections/connectionfriendlyname', ]);

requestsSearchRequest1Query = SearchQuery();
requestsSearchRequest1Query.setQueryString('contoso product');


requestsSearchRequest1.setQuery($requestsSearchRequest1Query);
requestsSearchRequest1.setFrom(0);

requestsSearchRequest1.setSize(25);

requestsSearchRequest1.setFields(['title', 'description', ]);


requestsArray []= requestsSearchRequest1;
requestBody.setRequests(requestsArray);




requestResult = graphServiceClient.search().query().post(requestBody);


```