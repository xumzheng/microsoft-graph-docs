---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackage();


$requestRequestBody->setCatalogId('aa2f6514-3232-46e7-a08a-2411ad8d7128');
$requestRequestBody->setDisplayName('sales reps');
$requestRequestBody->setDescription('outside sales representatives');
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackages()->post($requestRequestBody);


```