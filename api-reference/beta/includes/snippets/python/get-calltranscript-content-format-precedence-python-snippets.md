---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ContentRequestBuilderGetRequestConfiguration();

query_params = ContentRequestBuilderGetQueryParameters();
query_params.format = "text/vtt";

headers = [
'Accept' => 'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


awaitclient.usersById('user-id').onlineMeetingsById('onlineMeeting-id').transcriptsById('callTranscript-id').content().get(request_config);


```