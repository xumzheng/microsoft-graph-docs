---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PermissionGrantConditionSet();
requestBody.setPermissionType(PermissionType('delegated'));

requestBody.setClientApplicationsFromVerifiedPublisherOnly(true);



result = await client.policies().permissionGrantPoliciesById('permissionGrantPolicy-id').includes().post(requestBody);


```