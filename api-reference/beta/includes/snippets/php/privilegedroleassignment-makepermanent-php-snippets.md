---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MakePermanentPostRequestBody();


$requestRequestBody->setReason('reason-value');
$requestRequestBody->setTicketNumber('ticketNumber-value');
$requestRequestBody->setTicketSystem('ticketSystem-value');
$result =  $graphClient->privilegedRoleAssignmentsById('privilegedRoleAssignment-id')->makePermanent()->post($requestRequestBody);


```