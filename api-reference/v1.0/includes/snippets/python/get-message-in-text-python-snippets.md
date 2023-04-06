---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessageRequestBuilderGetRequestConfiguration(
request_config = MessageRequestBuilderGetRequestConfiguration(query_params=query_params = MessageRequestBuilderGetQueryParameters()
query_params.select = ["subject","body","bodyPreview","uniqueBody"]

)
query_params = MessageRequestBuilderGetQueryParameters()
query_params.select = ["subject","body","bodyPreview","uniqueBody"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.messages_by_id('message-id').get(request_config, headers=request_config)


```