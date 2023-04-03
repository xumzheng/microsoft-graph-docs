---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PermissionGrantConditionSet();
requestBody.setPermissionType(PermissionType('delegated'));

requestBody.setCertifiedClientApplicationsOnly(true);



result = awaitclient.policies().permissionGrantPoliciesById('permissionGrantPolicy-id').includes().post(requestBody);


```