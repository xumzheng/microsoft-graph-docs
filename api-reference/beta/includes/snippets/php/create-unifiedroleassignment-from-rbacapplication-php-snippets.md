---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignment();


$requestRequestBody->setRoleDefinitionId('c2cf284d-6c41-4e6b-afac-4b80928c9034');
$requestRequestBody->setPrincipalId('f8ca5a85-489a-49a0-b555-0a6d81e56f0d');
$requestRequestBody->setDirectoryScopeId('/');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.unifiedRoleAssignment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->roleManagement()->directory()->roleAssignments()->post($requestRequestBody);


```