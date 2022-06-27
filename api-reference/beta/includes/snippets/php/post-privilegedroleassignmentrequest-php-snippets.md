---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrivilegedRoleAssignmentRequest();


$requestRequestBody->setDuration('2');
$requestRequestBody->setReason('Activate the role for business purpose');
$requestRequestBody->setTicketNumber('234');
$requestRequestBody->setTicketSystem('system');

$schedule = new GovernanceSchedule();
$requestRequestBody->setSchedule($schedule);


$schedule->setStartDateTime(new DateTime("2018-02-08T02:35:17.903Z"));

$requestRequestBody->setType('UserAdd');
$requestRequestBody->setAssignmentState('Active');
$requestRequestBody->setRoleId('88d8e3e3-8f55-4a1e-953a-9b9898b8876b');
$result =  $graphClient->privilegedRoleAssignmentRequests()->post($requestRequestBody);


```