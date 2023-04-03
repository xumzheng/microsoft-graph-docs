---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = IdentityUserFlowAttributeAssignment();
requestBody.setIsOptional(false);

requestBody.setRequiresVerification(false);

requestBody.setUserInputType(IdentityUserFlowAttributeInputType('textbox'));

requestBody.setDisplayName('Shoe size');

requestBody.setUserAttributeValues([]);

userAttribute = IdentityUserFlowAttribute();
userAttribute.setId('extension_guid_shoeSize');


requestBody.setUserAttribute($userAttribute);


result = awaitclient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').userAttributeAssignments().post(requestBody);


```