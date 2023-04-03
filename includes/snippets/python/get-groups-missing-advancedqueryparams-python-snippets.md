---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = GroupsRequestBuilderGetRequestConfiguration();

queryParameters = GroupsRequestBuilderGetQueryParameters();
queryParameters.filter = "createdDateTime ge 2021-11-01";
queryParameters.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.groups().get(requestConfiguration);


```