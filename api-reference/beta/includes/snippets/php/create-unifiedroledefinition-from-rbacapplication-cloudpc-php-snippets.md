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

$rolePermissionsrolePermissions1 = new UnifiedRolePermission();

$rolePermissionsrolePermissions1AdditionalData = [
	"allowedResourceActions" => ['Microsoft.CloudPC/CloudPCs/Read',],
];
$rolePermissionsrolePermissions1->setAdditionalData($rolePermissionsrolePermissions1AdditionalData);

$rolePermissionsArray []= $rolePermissionsrolePermissions1;
$requestRequestBody->setRolePermissions($rolePermissionsArray);
$requestRequestBodyAdditionalData = [
"condition" => 'null',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->roleManagement()->cloudPC()->roleDefinitions()->post($requestRequestBody);


```