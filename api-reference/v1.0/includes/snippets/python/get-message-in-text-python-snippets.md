---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessageRequestBuilderGetRequestConfiguration(
request_config = MessageRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["subject","body","bodyPreview","uniqueBody"]
)
headers['Prefer'] = "outlook.body-content-type=\"text\""


result = await client.me.messages_by_id('message-id').get(request_config, headers=request_config)


```