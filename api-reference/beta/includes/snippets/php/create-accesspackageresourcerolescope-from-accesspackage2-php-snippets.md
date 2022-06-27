---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageResourceRoleScope();



$accessPackageResourceRole = new AccessPackageResourceRole();
$requestRequestBody->setAccessPackageResourceRole($accessPackageResourceRole);


$accessPackageResourceRole->setOriginId('4');
$accessPackageResourceRole->setOriginSystem('SharePointOnline');

$accessPackageResource = new AccessPackageResource();
$accessPackageResourceRole->setAccessPackageResource($accessPackageResource);


$accessPackageResource->setId('53c71803-a0a8-4777-aecc-075de8ee3991');



$accessPackageResourceScope = new AccessPackageResourceScope();
$requestRequestBody->setAccessPackageResourceScope($accessPackageResourceScope);


$accessPackageResourceScope->setId('5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33');
$accessPackageResourceScope->setOriginId('https://microsoft.sharepoint.com/portals/Community');
$accessPackageResourceScope->setOriginSystem('SharePointOnline');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackagesById('accessPackage-id')->accessPackageResourceRoleScopes()->post($requestRequestBody);


```