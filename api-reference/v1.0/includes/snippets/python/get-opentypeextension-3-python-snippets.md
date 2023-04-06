---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MessageRequestBuilderGetRequestConfiguration(
request_configuration = MessageRequestBuilderGetRequestConfiguration(query_params=query_params = MessageRequestBuilderGetQueryParameters()
query_params['expand'] = ["extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')"]

)
query_params = MessageRequestBuilderGetQueryParameters()
query_params['expand'] = ["extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')"]

)


result = await client.me.messages_by_id('message-id').get(request_configuration)


```