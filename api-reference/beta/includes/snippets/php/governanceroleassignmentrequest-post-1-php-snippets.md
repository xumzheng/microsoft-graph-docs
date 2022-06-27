---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GovernanceRoleAssignmentRequest();


$requestRequestBody->setRoleDefinitionId('ea48ad5e-e3b0-4d10-af54-39a45bbfe68d');
$requestRequestBody->setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5');
$requestRequestBody->setSubjectId('918e54be-12c4-4f4c-a6d3-2ee0e3661c51');
$requestRequestBody->setAssignmentState('Eligible');
$requestRequestBody->setType('AdminAdd');
$requestRequestBody->setReason('Assign an eligible role');

$schedule = new GovernanceSchedule();
$requestRequestBody->setSchedule($schedule);


$schedule->setStartDateTime(new DateTime("2018-05-12T23:37:43.356Z"));
$schedule->setEndDateTime(new DateTime("2018-11-08T23:37:43.356Z"));
$schedule->setType('Once');

$result =  $graphClient->privilegedAccessById('privilegedAccess-id')->roleAssignmentRequests()->post($requestRequestBody);


```