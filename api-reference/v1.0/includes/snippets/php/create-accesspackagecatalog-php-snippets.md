---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageCatalog();


$requestRequestBody->setDisplayName('sales');
$requestRequestBody->setDescription('for employees working with sales and outside sales partners');
$requestRequestBody->setState(new AccessPackageCatalogState('published'));
$requestRequestBody->setIsExternallyVisible(True);
$result =  $graphClient->identityGovernance()->entitlementManagement()->catalogs()->post($requestRequestBody);


```