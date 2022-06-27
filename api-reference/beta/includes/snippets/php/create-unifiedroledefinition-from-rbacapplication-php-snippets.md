---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleDefinition();


$requestRequestBody->setDescription('Update basic properties of application registrations');
$requestRequestBody->setDisplayName('Application Registration Support Administrator');
$rolePermissionsArray = [];

$rolePermissionsrolePermissions1 = new UnifiedRolePermission();

$rolePermissionsrolePermissions1AdditionalData = [
	"allowedResourceActions" => ['microsoft.directory/applications/basic/read',],
];
$rolePermissionsrolePermissions1->setAdditionalData($rolePermissionsrolePermissions1AdditionalData);

$rolePermissionsArray []= $rolePermissionsrolePermissions1;
$requestRequestBody->setRolePermissions($rolePermissionsArray);
$requestRequestBody->setIsEnabled('true');
$result =  $graphClient->roleManagement()->directory()->roleDefinitions()->post($requestRequestBody);


```