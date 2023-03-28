---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReferenceCreate();
$requestBody->set@odataid('https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2');



$graphServiceClient->identityGovernance()->entitlementManagement()->accessPackagesById('accessPackage-id')->incompatibleAccessPackages()->ref()->post($requestBody);


```