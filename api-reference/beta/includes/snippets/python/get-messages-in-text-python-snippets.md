---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
request_configuration = MessagesRequestBuilderGetRequestConfiguration(query_params=query_params = MessagesRequestBuilderGetQueryParameters()
query_params['select'] = ["subject","body","bodyPreview","uniqueBody"]

)
query_params = MessagesRequestBuilderGetQueryParameters()
query_params['select'] = ["subject","body","bodyPreview","uniqueBody"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.messages.get(request_configuration)


```