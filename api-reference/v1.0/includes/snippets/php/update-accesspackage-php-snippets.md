---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackage();


$requestRequestBody->setDisplayName('Access Package New Name');
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackagesById('accessPackage-id')->patch($requestRequestBody);


```