---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GovernanceRoleAssignmentRequest();


$requestRequestBody->setRoleDefinitionId('65bb4622-61f5-4f25-9d75-d0e20cf92019');
$requestRequestBody->setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5');
$requestRequestBody->setSubjectId('74765671-9ca4-40d7-9e36-2f4a570608a6');
$requestRequestBody->setAssignmentState('Eligible');
$requestRequestBody->setType('AdminRemove');
$result =  $graphClient->privilegedAccessById('privilegedAccess-id')->roleAssignmentRequests()->post($requestRequestBody);


```