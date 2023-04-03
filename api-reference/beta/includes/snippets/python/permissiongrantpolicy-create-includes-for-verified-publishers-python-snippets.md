---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PermissionGrantConditionSet();
requestBody.setPermissionType(PermissionType('delegated'));

requestBody.setClientApplicationsFromVerifiedPublisherOnly(true);



requestResult = graphServiceClient.policies().permissionGrantPoliciesById('permissionGrantPolicy-id').includes().post(requestBody);


```