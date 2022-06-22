---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityUserFlowAttributeAssignment();


$requestRequestBody->setIsOptional(False);
$requestRequestBody->setRequiresVerification(False);
$requestRequestBody->setUserInputType(new IdentityUserFlowAttributeInputType('TextBox'));
$requestRequestBody->setDisplayName('Shoe size');
$userAttributeValuesArray = [];
$requestRequestBody->setUserAttributeValues($userAttributeValuesArray);

$userAttribute = new IdentityUserFlowAttribute();
$requestRequestBody->setUserAttribute($userAttribute);


$userAttribute->setId('extension_guid_shoeSize');

$result =  $graphClient->identity()->b2xUserFlowsById('b2xIdentityUserFlow-id')->userAttributeAssignments()->post($requestRequestBody);


```