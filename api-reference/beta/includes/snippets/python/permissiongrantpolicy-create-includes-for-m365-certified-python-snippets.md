---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PermissionGrantConditionSet();
$requestBody.setPermissionType(new PermissionType('delegated'));

$requestBody.setCertifiedClientApplicationsOnly(true);



$requestResult = $graphServiceClient.policies().permissionGrantPoliciesById('permissionGrantPolicy-id').includes().post($requestBody);


```