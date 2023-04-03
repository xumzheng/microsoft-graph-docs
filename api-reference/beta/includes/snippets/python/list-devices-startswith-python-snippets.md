---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DevicesRequestBuilderGetRequestConfiguration();

queryParameters = DevicesRequestBuilderGetQueryParameters();
queryParameters.filter = "startswith(displayName,%20'a')";
queryParameters.count = true;
queryParameters.top = 1;
queryParameters.orderby = ["displayName"];

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.devices().get(requestConfiguration);


```