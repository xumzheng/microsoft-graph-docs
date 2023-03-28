---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AccessPackageCatalog();
$requestBody->setDisplayName('sales');

$requestBody->setDescription('for employees working with sales and outside sales partners');

$requestBody->setState(new AccessPackageCatalogState('published'));

$requestBody->setIsExternallyVisible(true);



$requestResult = $graphServiceClient->identityGovernance()->entitlementManagement()->catalogs()->post($requestBody);


```