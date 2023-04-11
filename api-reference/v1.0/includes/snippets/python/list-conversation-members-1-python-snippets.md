---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = MembersRequestBuilderGetRequestConfiguration(
)


result = await client.me.chats_by_id('chat-id').members.get()


```