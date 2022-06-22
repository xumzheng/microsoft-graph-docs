---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignmentMultiple();


$requestRequestBody->setDisplayName('My test role assignment 1');
$requestRequestBody->setRoleDefinitionId('c2cf284d-6c41-4e6b-afac-4b80928c9034');
$requestRequestBody->setPrincipalIds( [
'f8ca5a85-489a-49a0-b555-0a6d81e56f0d','c1518aa9-4da5-4c84-a902-a31404023890',],
$requestRequestBody->setDirectoryScopeIds( [
'28ca5a85-489a-49a0-b555-0a6d81e56f0d','8152656a-cf9a-4928-a457-1512d4cae295',],
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.unifiedRoleAssignmentMultiple',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->roleManagement()->deviceManagement()->roleAssignments()->post($requestRequestBody);


```