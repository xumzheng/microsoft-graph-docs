---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessagesRequestBuilderGetRequestConfiguration(
request_configuration = MessagesRequestBuilderGetRequestConfiguration(query_params=query_params = MessagesRequestBuilderGetQueryParameters()
query_params['filter'] = "Extensions/any"
query_params['expand'] = ["Extensions($filter=id%20eq%20'Com.Contoso.Referral')"]

)
query_params = MessagesRequestBuilderGetQueryParameters()
query_params['filter'] = "Extensions/any"
query_params['expand'] = ["Extensions($filter=id%20eq%20'Com.Contoso.Referral')"]

)


result = await client.me.messages.get(request_configuration)


```