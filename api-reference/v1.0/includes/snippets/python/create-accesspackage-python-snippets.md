---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AccessPackage();
$requestBody.setDisplayName('sales reps');

$requestBody.setDescription('outside sales representatives');

$requestBody.setIsHidden(false);

$catalog = new AccessPackageCatalog();
$catalog.setId('66584aae-98bb-48cc-9458-7bee5d2a6577');


$requestBody.setCatalog($catalog);


$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().accessPackages().post($requestBody);


```