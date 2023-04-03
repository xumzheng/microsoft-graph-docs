---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = GroupRequestBuilderGetRequestConfiguration();

queryParameters = GroupRequestBuilderGetQueryParameters();
queryParameters.count = true;
queryParameters.orderby = ["displayName"];
queryParameters.filter = "startswith(displayName,%20'A')";

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.groupsById('group-id').memberOf().graphGroup().get(requestConfiguration);


```