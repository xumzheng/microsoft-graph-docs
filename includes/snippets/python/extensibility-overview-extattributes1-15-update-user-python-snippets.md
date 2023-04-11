---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
onPremisesExtensionAttributes = OnPremisesExtensionAttributes()
onPremisesExtensionAttributes.extensionAttribute1 = 'skypeId.adeleVance'

OnPremisesExtensionAttributes.extensionAttribute13=null


request_body.onPremisesExtensionAttributes = onPremisesExtensionAttributes


request_configuration = UserRequestBuilderPatchRequestConfiguration(
)


result = await client.users_by_id('user-id').patch(request_body = request_body)


```