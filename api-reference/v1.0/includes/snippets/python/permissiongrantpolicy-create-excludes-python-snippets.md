---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PermissionGrantConditionSet();
$requestBody->setPermissionType(new PermissionType('delegated'));

$requestBody->setResourceApplication('00000003-0000-0000-c000-000000000000');



$requestResult = $graphServiceClient->policies()->permissionGrantPoliciesById('permissionGrantPolicy-id')->excludes()->post($requestBody);


```