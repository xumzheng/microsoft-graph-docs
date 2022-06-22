---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleEligibilityScheduleRequest();


$requestRequestBody->setAction(new UnifiedRoleScheduleRequestActions('adminAssign'));
$requestRequestBody->setJustification('Assign Attribute Assignment Admin eligibility to restricted user');
$requestRequestBody->setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4');
$requestRequestBody->setDirectoryScopeId('/');
$requestRequestBody->setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');

$scheduleInfo = new RequestSchedule();
$requestRequestBody->setScheduleInfo($scheduleInfo);


$scheduleInfo->setStartDateTime(new DateTime("2022-04-10T00:00:00Z"));

$expiration = new ExpirationPattern();
$scheduleInfo->setExpiration($expiration);


$expiration->setType(new ExpirationPatternType('afterDateTime'));
$expiration->setEndDateTime(new DateTime("2024-04-10T00:00:00Z"));


$result =  $graphClient->roleManagement()->directory()->roleEligibilityScheduleRequests()->post($requestRequestBody);


```