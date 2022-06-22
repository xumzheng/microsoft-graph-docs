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

$rolePermissions1 = new UnifiedRolePermission();

$rolePermissions1AdditionalData = [
		"allowedResourceActions" =>  [
'microsoft.directory/applications/basic/read',		],
	];
$rolePermissions1->setAdditionalData($rolePermissions1AdditionalData);

$rolePermissionsArray []= $rolePermissions1;
$requestRequestBody->setRolePermissions($rolePermissionsArray);
$requestRequestBody->setIsEnabled(True);
$result =  $graphClient->roleManagement()->directory()->roleDefinitions()->post($requestRequestBody);


```