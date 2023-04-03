---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DevicesRequestBuilderGetRequestConfiguration();

queryParameters = DevicesRequestBuilderGetQueryParameters();
queryParameters.search = "\"displayName:Android\"";
queryParameters.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.devices().get(requestConfiguration);


```