---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignment();


$requestRequestBody->setRoleDefinitionId('58a13ea3-c632-46ae-9ee0-9c0d43cd7f3d');
$requestRequestBody->setPrincipalId('f8ca5a85-489a-49a0-b555-0a6d81e56f0d');
$requestRequestBody->setDirectoryScopeId('/attributeSets/Engineering');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.unifiedRoleAssignment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->roleManagement()->directory()->roleAssignments()->post($requestRequestBody);


```