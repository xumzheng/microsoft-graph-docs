---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration(
request_config = MessagesRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "MentionsPreview/IsMentioned eq true"
params['select'] = ["Subject","Sender","ReceivedDateTime","MentionsPreview"]
)


result = await client.me.messages.get(request_config, headers=request_config)


```