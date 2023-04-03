---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PermissionGrantPolicy();
requestBody.setDisplayName('Custom permission grant policy');



result = awaitclient.policies().permissionGrantPoliciesById('permissionGrantPolicy-id').patch(requestBody);


```