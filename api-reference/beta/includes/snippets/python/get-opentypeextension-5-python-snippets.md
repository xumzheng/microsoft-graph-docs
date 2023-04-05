---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MessagesRequestBuilderGetRequestConfiguration()

query_params = MessagesRequestBuilderGetQueryParameters()
query_params.filter = "Extensions/any"
query_params.expand = ["Extensions($filter=id%20eq%20'Com.Contoso.Referral')"]

request_config.queryParameters = query_params


result = await client.me.messages.get(request_config)


```