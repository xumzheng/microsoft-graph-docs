---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MeRequestBuilderGetRequestConfiguration();

queryParameters = MeRequestBuilderGetQueryParameters();
queryParameters.expand = ["manager($levels=max;$select=id,displayName)"];
queryParameters.select = ["id","displayName"];

headers = [
'ConsistencyLevel' => 'eventual',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().get(requestConfiguration);


```