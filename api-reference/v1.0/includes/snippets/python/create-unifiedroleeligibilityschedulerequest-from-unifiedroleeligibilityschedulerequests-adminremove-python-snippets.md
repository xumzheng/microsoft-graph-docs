---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnifiedRoleEligibilityScheduleRequest();
$requestBody->setAction('adminRemove');

$requestBody->setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4');

$requestBody->setDirectoryScopeId('/');

$requestBody->setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b');



$requestResult = $graphServiceClient->roleManagement()->directory()->roleEligibilityScheduleRequests()->post($requestBody);


```