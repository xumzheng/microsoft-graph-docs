---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleEligibilityScheduleRequest();


$requestRequestBody->setAction('adminRemove');
$requestRequestBody->setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4');
$requestRequestBody->setDirectoryScopeId('/');
$requestRequestBody->setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');
$result =  $graphClient->roleManagement()->directory()->roleEligibilityScheduleRequests()->post($requestRequestBody);


```