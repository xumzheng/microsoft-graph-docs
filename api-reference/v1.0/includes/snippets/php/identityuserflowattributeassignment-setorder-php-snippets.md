---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new NewAssignmentOrderRequestBody();



$newAssignmentOrder = new AssignmentOrder();
$requestRequestBody->setNewAssignmentOrder($newAssignmentOrder);


$newAssignmentOrder->setOrder(['City','extension_GUID_ShoeSize',]);

$result =  $graphClient->identity()->b2xUserFlowsById('b2xIdentityUserFlow-id')->userAttributeAssignments()->setOrder()->post($requestRequestBody);


```