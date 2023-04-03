---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = GroupsRequestBuilderGetRequestConfiguration();

queryParameters = GroupsRequestBuilderGetQueryParameters();
queryParameters.search = "\"displayName:Video\" OR \"description:prod\"";
queryParameters.orderby = ["displayName"];
queryParameters.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.groups().get(requestConfiguration);


```