---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleAssignment();


$requestRequestBody->setPrincipalId('6b937a9d-c731-465b-a844-2d5b5368c161');
$requestRequestBody->setRoleDefinitionId('9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3');
$requestRequestBody->setDirectoryScopeId('/661e1310-bd76-4795-89a7-8f3c8f855bfc');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.unifiedRoleAssignment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->roleManagement()->directory()->roleAssignments()->post($requestRequestBody);


```