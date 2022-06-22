---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackage();


$requestRequestBody->setDisplayName('sales reps');
$requestRequestBody->setDescription('outside sales representatives');
$requestRequestBody->setIsHidden(False);

$catalog = new AccessPackageCatalog();
$requestRequestBody->setCatalog($catalog);


$catalog->setId('66584aae-98bb-48cc-9458-7bee5d2a6577');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackages()->post($requestRequestBody);


```