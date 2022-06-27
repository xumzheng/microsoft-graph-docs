---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignmentMultiple();


$requestRequestBody->setDisplayName('NewName');
$requestRequestBody->setDescription('A new roleAssignment');
$result =  $graphClient->roleManagement()->cloudPC()->roleAssignmentsById('unifiedRoleAssignmentMultiple-id')->patch($requestRequestBody);


```