---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemAddress()
request_body.setAllowedAudiences(AllowedAudiences('me'))

request_body.setDisplayName('Secret Hideout')


request_config = ItemAddressRequestBuilderPatchRequestConfiguration(
request_config = ItemAddressRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.users_by_id('user-id').profile.addresses_by_id('itemAddress-id').patch(request_body, headers=)


```