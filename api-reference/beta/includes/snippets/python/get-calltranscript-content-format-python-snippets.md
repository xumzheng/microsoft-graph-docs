---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ContentRequestBuilderGetRequestConfiguration();

query_params = ContentRequestBuilderGetQueryParameters();
query_params.format = "text/vtt";

request_config.queryParameters = query_params;


awaitclient.usersById('user-id').onlineMeetingsById('onlineMeeting-id').transcriptsById('callTranscript-id').content().get(request_config);


```