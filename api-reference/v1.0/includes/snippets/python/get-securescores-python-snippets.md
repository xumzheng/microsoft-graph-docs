---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = SecureScoresRequestBuilderGetRequestConfiguration();

query_params = SecureScoresRequestBuilderGetQueryParameters;
query_params.top = 1;

request_config.queryParameters = query_params;


result = await client.security().secureScores().get(request_config);


```