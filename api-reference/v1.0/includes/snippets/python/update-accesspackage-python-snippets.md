---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AccessPackage();
$requestBody.setDisplayName('Access Package New Name');



$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().accessPackagesById('accessPackage-id').patch($requestBody);


```