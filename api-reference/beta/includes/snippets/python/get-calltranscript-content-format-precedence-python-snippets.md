---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ContentRequestBuilderGetRequestConfiguration()

query_params = ContentRequestBuilderGetQueryParameters()
query_params.format = "text/vtt"

headers = [
'Accept' => 'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
]

request_config.queryParameters = query_params
request_config.headers = headers


await client.usersby_id('user-id')_onlineMeetingsby_id('onlineMeeting-id')_transcriptsby_id('callTranscript-id')_content.get(request_config)


```