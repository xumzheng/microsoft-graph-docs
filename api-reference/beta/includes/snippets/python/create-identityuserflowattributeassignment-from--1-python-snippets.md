---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityUserFlowAttributeAssignment();
$requestBody->setIsOptional(false);

$requestBody->setRequiresVerification(false);

$requestBody->setUserInputType(new IdentityUserFlowAttributeInputType('textbox'));

$requestBody->setDisplayName('Shoe size');

$requestBody->setUserAttributeValues([]);

$userAttribute = new IdentityUserFlowAttribute();
$userAttribute->setId('extension_guid_shoeSize');


$requestBody->setUserAttribute($userAttribute);


$requestResult = $graphServiceClient->identity()->b2cUserFlowsById('b2cIdentityUserFlow-id')->userAttributeAssignments()->post($requestBody);


```