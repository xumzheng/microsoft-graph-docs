---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignmentScheduleRequest();


$requestRequestBody->setAction('SelfActivate');
$requestRequestBody->setPrincipalId('c6ad1942-4afa-47f8-8d48-afb5d8d69d2f');
$requestRequestBody->setRoleDefinitionId('9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3');
$requestRequestBody->setDirectoryScopeId('/');
$requestRequestBody->setJustification('Need to update app roles for selected apps.');

$scheduleInfo = new RequestSchedule();
$requestRequestBody->setScheduleInfo($scheduleInfo);


$scheduleInfo->setStartDateTime(new DateTime("2021-08-17T17:40:00.000Z"));

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