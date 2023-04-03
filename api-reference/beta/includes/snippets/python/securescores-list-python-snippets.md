---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = SecureScoresRequestBuilderGetRequestConfiguration();

queryParameters = SecureScoresRequestBuilderGetQueryParameters();
queryParameters.top = 1;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.security().secureScores().get(requestConfiguration);


```