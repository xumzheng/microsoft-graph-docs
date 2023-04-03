---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthorizationPolicy();
requestBody.setEnabledPreviewFeatures(['assignGroupsToRoles', ]);



result = awaitclient.policies().authorizationPolicyById('authorizationPolicy-id').patch(requestBody);


```