---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttributeAssignment()
request_body.is_optional = False

request_body.requires_verification = False

request_body.UserInputType(IdentityUserFlowAttributeInputType('textbox'))

request_body.displayName = 'Shoe size'

request_body.UserAttributeValues([])

user_attribute = IdentityUserFlowAttribute()
userAttribute.id = 'extension_guid_shoeSize'


request_body.user_attribute = userAttribute



result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').userAttributeAssignments.post(request_body = request_body)


```