---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageResourceRequest();


$requestRequestBody->setCatalogId('beedadfe-01d5-4025-910b-84abb9369997');
$requestRequestBody->setRequestType('AdminRemove');

$accessPackageResource = new AccessPackageResource();
$requestRequestBody->setAccessPackageResource($accessPackageResource);


$accessPackageResource->setId('354078e5-dbce-4894-8af4-0ab274d41662');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageResourceRequests()->post($requestRequestBody);


```