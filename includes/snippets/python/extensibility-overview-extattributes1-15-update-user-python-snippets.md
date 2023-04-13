---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
on_premises_extension_attributes = OnPremisesExtensionAttributes()
onPremisesExtensionAttributes.extensionAttribute1 = 'skypeId.adeleVance'

OnPremisesExtensionAttributes.extensionAttribute13=null


request_body.on_premises_extension_attributes = onPremisesExtensionAttributes



result = await client.users_by_id('user-id').patch(request_body = request_body)


```