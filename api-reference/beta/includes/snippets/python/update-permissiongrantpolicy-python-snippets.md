---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PermissionGrantPolicy();
requestBody.setDisplayName('Custom permission grant policy');



requestResult = graphServiceClient.policies().permissionGrantPoliciesById('permissionGrantPolicy-id').patch(requestBody);


```