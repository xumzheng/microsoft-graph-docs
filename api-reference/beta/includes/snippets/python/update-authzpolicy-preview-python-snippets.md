---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AuthorizationPolicy();
requestBody.setEnabledPreviewFeatures(['assignGroupsToRoles', ]);



result = await client.policies().authorizationPolicyById('authorizationPolicy-id').patch(requestBody);


```