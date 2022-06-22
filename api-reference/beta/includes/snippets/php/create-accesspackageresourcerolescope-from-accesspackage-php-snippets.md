---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageResourceRoleScope();



$accessPackageResourceRole = new AccessPackageResourceRole();
$requestRequestBody->setAccessPackageResourceRole($accessPackageResourceRole);


$accessPackageResourceRole->setOriginId('Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca');
$accessPackageResourceRole->setDisplayName('Member');
$accessPackageResourceRole->setOriginSystem('AadGroup');

$accessPackageResource = new AccessPackageResource();
$accessPackageResourceRole->setAccessPackageResource($accessPackageResource);


$accessPackageResource->setId('1d08498d-72a1-403f-8511-6b1f875746a0');
$accessPackageResource->setResourceType('O365 Group');
$accessPackageResource->setOriginId('b31fe1f1-3651-488f-bd9a-1711887fd4ca');
$accessPackageResource->setOriginSystem('AadGroup');



$accessPackageResourceScope = new AccessPackageResourceScope();
$requestRequestBody->setAccessPackageResourceScope($accessPackageResourceScope);


$accessPackageResourceScope->setOriginId('b31fe1f1-3651-488f-bd9a-1711887fd4ca');
$accessPackageResourceScope->setOriginSystem('AadGroup');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackagesById('accessPackage-id')->accessPackageResourceRoleScopes()->post($requestRequestBody);


```