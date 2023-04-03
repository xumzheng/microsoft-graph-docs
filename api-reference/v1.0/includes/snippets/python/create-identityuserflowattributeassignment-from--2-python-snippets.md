---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IdentityUserFlowAttributeAssignment();
requestBody.setIsOptional(false);

requestBody.setRequiresVerification(false);

requestBody.setUserInputType(IdentityUserFlowAttributeInputType('textbox'));

requestBody.setDisplayName('Shoe size');

requestBody.setUserAttributeValues([]);

userAttribute = IdentityUserFlowAttribute();
userAttribute.setId('extension_guid_shoeSize');


requestBody.setUserAttribute($userAttribute);


result = await client.identity().b2xUserFlowsById('b2xIdentityUserFlow-id').userAttributeAssignments().post(requestBody);


```