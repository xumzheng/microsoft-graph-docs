---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = MessageRequestBuilder.MessageRequestBuilderGetQueryParameters(
				expand = ["extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')"],
)

request_configuration = MessageRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.me.messages_by_id('message-id').get(request_configuration = request_configuration)


```