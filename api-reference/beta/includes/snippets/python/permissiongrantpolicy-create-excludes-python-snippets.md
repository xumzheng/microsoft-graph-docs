---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PermissionGrantConditionSet();
requestBody.setPermissionType(PermissionType('delegated'));

requestBody.setResourceApplication('00000003-0000-0000-c000-000000000000');



result = await client.policies().permissionGrantPoliciesById('permissionGrantPolicy-id').excludes().post(requestBody);


```