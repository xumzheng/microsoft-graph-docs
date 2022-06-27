---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GovernanceRoleAssignmentRequest();


$requestRequestBody->setRoleDefinitionId('0e88fd18-50f5-4ee1-9104-01c3ed910065');
$requestRequestBody->setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5');
$requestRequestBody->setSubjectId('74765671-9ca4-40d7-9e36-2f4a570608a6');
$requestRequestBody->setAssignmentState('Eligible');
$requestRequestBody->setType('AdminExtend');
$requestRequestBody->setReason('extend role assignment');

$schedule = new GovernanceSchedule();
$requestRequestBody->setSchedule($schedule);


$schedule->setType('Once');
$schedule->setStartDateTime(new DateTime("2018-05-12T23:53:55.327Z"));
$schedule->setEndDateTime(new DateTime("2018-08-10T23:53:55.327Z"));

$result =  $graphClient->privilegedAccessById('privilegedAccess-id')->roleAssignmentRequests()->post($requestRequestBody);


```