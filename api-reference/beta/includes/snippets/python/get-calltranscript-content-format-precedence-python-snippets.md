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


await client.users._by_id('user-id').onlineMeetings._by_id('onlineMeeting-id').transcripts._by_id('callTranscript-id').content.get(request_config)


```