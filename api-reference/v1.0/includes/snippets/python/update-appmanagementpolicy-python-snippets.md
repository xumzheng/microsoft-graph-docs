---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AppManagementPolicy();
requestBody.setIsEnabled(false);



requestResult = graphServiceClient.policies().appManagementPoliciesById('appManagementPolicy-id').patch(requestBody);


```