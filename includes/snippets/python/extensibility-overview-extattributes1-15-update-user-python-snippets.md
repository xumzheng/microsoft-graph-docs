---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
onPremisesExtensionAttributes = OnPremisesExtensionAttributes()
onPremisesExtensionAttributes.setExtensionAttribute1('skypeId.adeleVance')

OnPremisesExtensionAttributes.setExtensionAttribute13(null)


request_body.setOnPremisesExtensionAttributes($onPremisesExtensionAttributes)


result = await client.users_by_id('user-id').patch(request_body)


```