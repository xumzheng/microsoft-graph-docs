---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = ChatMessageRequestBuilderGetRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').get()


```