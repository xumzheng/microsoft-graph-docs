---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = OnlineMeetingsRequestBuilderGetRequestConfiguration();

query_params = OnlineMeetingsRequestBuilderGetQueryParameters();
query_params.filter = "joinMeetingIdSettings/joinMeetingId eq '1234567890'";

request_config.queryParameters = query_params;


result = awaitclient.me().onlineMeetings().get(request_config);


```