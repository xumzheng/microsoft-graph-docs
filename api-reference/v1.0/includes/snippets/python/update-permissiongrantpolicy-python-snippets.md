---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PermissionGrantPolicy();
requestBody.setDisplayName('Custom permission grant policy');



result = await client.policies().permissionGrantPoliciesById('permissionGrantPolicy-id').patch(requestBody);


```