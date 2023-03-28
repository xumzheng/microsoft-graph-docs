---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AccessPackage();
$requestBody->setCatalogId('cec5d6ab-c75d-47c0-9c1c-92e89f66e384');

$requestBody->setDisplayName('Marketing Campaign');

$requestBody->setDescription('Access to resources for the campaign');



$requestResult = $graphServiceClient->identityGovernance()->entitlementManagement()->accessPackages()->post($requestBody);


```