---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MeRequestBuilderGetRequestConfiguration();

queryParameters = MeRequestBuilderGetQueryParameters();
queryParameters.select = ["id","displayName","mail","mobilePhone"];
queryParameters.expand = ["extensions"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().get(requestConfiguration);


```