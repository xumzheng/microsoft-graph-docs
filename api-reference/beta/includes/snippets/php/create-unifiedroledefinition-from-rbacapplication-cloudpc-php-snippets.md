---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleDefinition();


$requestRequestBody->setDescription('An example custom role');
$requestRequestBody->setDisplayName('ExampleCustomRole');
$rolePermissionsArray = [];

$rolePermissions1 = new UnifiedRolePermission();

$rolePermissions1AdditionalData = [
		"allowedResourceActions" =>  [
'Microsoft.CloudPC/CloudPCs/Read',		],
	];
$rolePermissions1->setAdditionalData($rolePermissions1AdditionalData);

$rolePermissionsArray []= $rolePermissions1;
$requestRequestBody->setRolePermissions($rolePermissionsArray);
$requestRequestBodyAdditionalData = [
"condition" => 'null',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->roleManagement()->cloudPC()->roleDefinitions()->post($requestRequestBody);


```