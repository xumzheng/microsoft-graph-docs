---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignmentScheduleRequest();


$requestRequestBody->setAction(new UnifiedRoleScheduleRequestActions('adminAssign'));
$requestRequestBody->setJustification('Assign Groups Admin to IT Helpdesk group');
$requestRequestBody->setRoleDefinitionId('fdd7a751-b60b-444a-984c-02652fe8fa1c');
$requestRequestBody->setDirectoryScopeId('/');
$requestRequestBody->setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');

$scheduleInfo = new RequestSchedule();
$requestRequestBody->setScheduleInfo($scheduleInfo);


$scheduleInfo->setStartDateTime(new DateTime("2022-04-10T00:00:00Z"));

$expiration = new ExpirationPattern();
$scheduleInfo->setExpiration($expiration);


$expiration->setType(new ExpirationPatternType('NoExpiration'));


$result =  $graphClient->roleManagement()->directory()->roleAssignmentScheduleRequests()->post($requestRequestBody);


```