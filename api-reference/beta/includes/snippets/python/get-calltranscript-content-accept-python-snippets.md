---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ContentRequestBuilderGetRequestConfiguration();

headers = [
	'Accept' => 'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
];

request_config.headers = headers;


awaitclient.usersById('user-id').onlineMeetingsById('onlineMeeting-id').transcriptsById('callTranscript-id').content().get(request_config);


```