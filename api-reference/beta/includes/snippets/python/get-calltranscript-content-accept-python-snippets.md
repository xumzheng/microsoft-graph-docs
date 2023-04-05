---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ContentRequestBuilderGetRequestConfiguration()

headers = [
	'Accept' => 'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
]

request_config.headers = headers


await client.users._by_id('user-id').onlineMeetings._by_id('onlineMeeting-id').transcripts._by_id('callTranscript-id').content.get(request_config)


```