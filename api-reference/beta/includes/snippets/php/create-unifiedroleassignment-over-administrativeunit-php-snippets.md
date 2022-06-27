---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignment();


$requestRequestBody->setRoleDefinitionId('fe930be7-5e62-47db-91af-98c3a49a38b1');
$requestRequestBody->setPrincipalId('f8ca5a85-489a-49a0-b555-0a6d81e56f0d');
$requestRequestBody->setDirectoryScopeId('/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.unifiedRoleAssignment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->roleManagement()->directory()->roleAssignments()->post($requestRequestBody);


```