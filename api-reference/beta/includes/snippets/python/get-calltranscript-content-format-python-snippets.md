---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ContentRequestBuilderGetRequestConfiguration(
request_config = ContentRequestBuilderGetRequestConfiguration(query_params=query_params = ContentRequestBuilderGetQueryParameters()
query_params.format = "text/vtt"

)
query_params = ContentRequestBuilderGetQueryParameters()
query_params.format = "text/vtt"

)


await client.users_by_id('user-id').onlineMeetings_by_id('onlineMeeting-id').transcripts_by_id('callTranscript-id').content.get(request_config, headers=request_config)


```