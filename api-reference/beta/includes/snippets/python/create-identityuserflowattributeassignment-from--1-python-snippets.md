---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttributeAssignment()
request_body.setIsOptional(false)

request_body.setRequiresVerification(false)

request_body.setUserInputType(IdentityUserFlowAttributeInputType('textbox'))

request_body.setDisplayName('Shoe size')

request_body.setUserAttributeValues([])

userAttribute = IdentityUserFlowAttribute()
userAttribute.setId('extension_guid_shoeSize')


request_body.setUserAttribute($userAttribute)


result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').userAttributeAssignments.post(request_body, headers=)


```