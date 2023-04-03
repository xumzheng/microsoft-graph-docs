---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = SecureScoresRequestBuilderGetRequestConfiguration();

query_params = SecureScoresRequestBuilderGetQueryParameters();
query_params.top = 1;

request_config.queryParameters = query_params;


result = awaitclient.security().secureScores().get(request_config);


```