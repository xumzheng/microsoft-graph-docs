---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GovernanceRoleAssignmentRequest();


$requestRequestBody->setRoleDefinitionId('8b4d1d51-08e9-4254-b0a6-b16177aae376');
$requestRequestBody->setResourceId('e5e7d29d-5465-45ac-885f-4716a5ee74b5');
$requestRequestBody->setSubjectId('918e54be-12c4-4f4c-a6d3-2ee0e3661c51');
$requestRequestBody->setAssignmentState('Active');
$requestRequestBody->setType('UserAdd');
$requestRequestBody->setReason('Activate the owner role');

$schedule = new GovernanceSchedule();
$requestRequestBody->setSchedule($schedule);


$schedule->setType('Once');
$schedule->setStartDateTime(new DateTime("2018-05-12T23:28:43.537Z"));
$schedule->setDuration('PT9H');

$requestRequestBody->setLinkedEligibleRoleAssignmentId('e327f4be-42a0-47a2-8579-0a39b025b394');
$result =  $graphClient->privilegedAccessById('privilegedAccess-id')->roleAssignmentRequests()->post($requestRequestBody);


```