---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleDefinition();


$requestRequestBody->setDescription('Update basic properties and permission of application registrations');
$requestRequestBody->setDisplayName('ExampleCustomRole');
$rolePermissionsArray = [];

$rolePermissionsrolePermissions1 = new UnifiedRolePermission();

$rolePermissionsrolePermissions1AdditionalData = [
	"allowedResourceActions" => ['Microsoft.CloudPC/CloudPCs/Read','Microsoft.CloudPC/CloudPCs/Reprovision',],
];
$rolePermissionsrolePermissions1->setAdditionalData($rolePermissionsrolePermissions1AdditionalData);

$rolePermissionsArray []= $rolePermissionsrolePermissions1;
$requestRequestBody->setRolePermissions($rolePermissionsArray);
$result =  $graphClient->roleManagement()->cloudPC()->roleDefinitionsById('unifiedRoleDefinition-id')->patch($requestRequestBody);


```