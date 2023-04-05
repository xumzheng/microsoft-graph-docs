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


await client.usersby_id('user-id')_onlineMeetingsby_id('onlineMeeting-id')_transcriptsby_id('callTranscript-id')_content.get(request_config)


```