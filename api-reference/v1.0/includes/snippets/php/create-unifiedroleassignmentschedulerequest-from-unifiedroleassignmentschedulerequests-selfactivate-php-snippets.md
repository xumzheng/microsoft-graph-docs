---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignmentScheduleRequest();


$requestRequestBody->setAction(new UnifiedRoleScheduleRequestActions('selfActivate'));
$requestRequestBody->setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');
$requestRequestBody->setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4');
$requestRequestBody->setDirectoryScopeId('/');
$requestRequestBody->setJustification('I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs');

$scheduleInfo = new RequestSchedule();
$requestRequestBody->setScheduleInfo($scheduleInfo);


$scheduleInfo->setStartDateTime(new DateTime("2022-04-14T00:00:00.000Z"));

$expiration = new ExpirationPattern();
$scheduleInfo->setExpiration($expiration);


$expiration->setType(new ExpirationPatternType('AfterDuration'));
$expiration->setDuration('PT5H');



$ticketInfo = new TicketInfo();
$requestRequestBody->setTicketInfo($ticketInfo);


$ticketInfo->setTicketNumber('CONTOSO:Normal-67890');
$ticketInfo->setTicketSystem('MS Project');

$result =  $graphClient->roleManagement()->directory()->roleAssignmentScheduleRequests()->post($requestRequestBody);


```