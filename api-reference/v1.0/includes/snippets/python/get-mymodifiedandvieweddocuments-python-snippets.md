---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = UsedRequestBuilderGetRequestConfiguration();

queryParameters = UsedRequestBuilderGetQueryParameters();
queryParameters.orderby = ["LastUsed/LastAccessedDateTime desc"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().insights().used().get(requestConfiguration);


```