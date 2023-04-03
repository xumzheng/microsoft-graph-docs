---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AppManagementPolicy();
requestBody.setIsEnabled(false);



result = awaitclient.policies().appManagementPoliciesById('appManagementPolicy-id').patch(requestBody);


```