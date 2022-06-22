---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageResourceRequest();


$requestRequestBody->setCatalogId('beedadfe-01d5-4025-910b-84abb9369997');
$requestRequestBody->setRequestType('AdminAdd');

$accessPackageResource = new AccessPackageResource();
$requestRequestBody->setAccessPackageResource($accessPackageResource);


$accessPackageResource->setOriginId('c6294667-7348-4f5a-be73-9d2c65f574f3');
$accessPackageResource->setOriginSystem('AadGroup');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageResourceRequests()->post($requestRequestBody);


```