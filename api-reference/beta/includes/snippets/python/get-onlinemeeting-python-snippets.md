---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = OnlineMeetingsRequestBuilderGetRequestConfiguration();

query_params = OnlineMeetingsRequestBuilderGetQueryParameters();
query_params.filter = "VideoTeleconferenceId eq '123456789'";

request_config.queryParameters = query_params;


result = awaitclient.communications().onlineMeetings().get(request_config);


```