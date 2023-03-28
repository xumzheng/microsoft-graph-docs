---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AccessPackage();
$requestBody->setCatalogId('aa2f6514-3232-46e7-a08a-2411ad8d7128');

$requestBody->setDisplayName('sales reps');

$requestBody->setDescription('outside sales representatives');



$requestResult = $graphServiceClient->identityGovernance()->entitlementManagement()->accessPackages()->post($requestBody);


```