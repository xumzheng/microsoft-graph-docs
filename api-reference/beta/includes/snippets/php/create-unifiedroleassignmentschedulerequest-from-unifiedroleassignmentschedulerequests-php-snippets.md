---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignmentScheduleRequest();


$requestRequestBody->setAction('AdminAssign');
$requestRequestBody->setJustification('Assign User Admin to IT Helpdesk (User) group');
$requestRequestBody->setRoleDefinitionId('fdd7a751-b60b-444a-984c-02652fe8fa1c');
$requestRequestBody->setDirectoryScopeId('/');
$requestRequestBody->setPrincipalId('07706ff1-46c7-4847-ae33-3003830675a1');

$scheduleInfo = new RequestSchedule();
$requestRequestBody->setScheduleInfo($scheduleInfo);


$scheduleInfo->setStartDateTime(new DateTime("2021-07-01T00:00:00Z"));

$expiration = new ExpirationPattern();
$scheduleInfo->setExpiration($expiration);


$expiration->setType(new ExpirationPatternType('NoExpiration'));


$result =  $graphClient->roleManagement()->directory()->roleAssignmentScheduleRequests()->post($requestRequestBody);


```