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

$rolePermissions1 = new UnifiedRolePermission();

$rolePermissions1AdditionalData = [
		"allowedResourceActions" =>  [
'Microsoft.CloudPC/CloudPCs/Read','Microsoft.CloudPC/CloudPCs/Reprovision',		],
	];
$rolePermissions1->setAdditionalData($rolePermissions1AdditionalData);

$rolePermissionsArray []= $rolePermissions1;
$requestRequestBody->setRolePermissions($rolePermissionsArray);
$result =  $graphClient->roleManagement()->cloudPC()->roleDefinitionsById('unifiedRoleDefinition-id')->patch($requestRequestBody);


```