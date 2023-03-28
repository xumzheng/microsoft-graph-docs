---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new QueryPostRequestBody();
$requestsSearchRequest1 = new SearchRequest();
$requestsSearchRequest1.setEntityTypes([$requestsSearchRequest1.setEntityType(new EntityType('chatmessage'));
]);

$requestsSearchRequest1Query = new SearchQuery();
$requestsSearchRequest1Query.setQueryString('test');


$requestsSearchRequest1.setQuery($requestsSearchRequest1Query);
$requestsSearchRequest1.setFrom(0);

$requestsSearchRequest1.setSize(25);


$requestsArray []= $requestsSearchRequest1;
$requestBody.setRequests($requestsArray);




$requestResult = $graphServiceClient.search().query().post($requestBody);


```