---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityUserFlowAttributeAssignment();


$requestRequestBody->setUserInputType(new IdentityUserFlowAttributeInputType('textBox'));
$result =  $graphClient->identity()->b2xUserFlowsById('b2xIdentityUserFlow-id')->userAttributeAssignmentsById('identityUserFlowAttributeAssignment-id')->patch($requestRequestBody);


```