---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PermissionGrantPolicy();
requestBody.setId('my-custom-consent-policy');

requestBody.setDisplayName('Custom application consent policy');

requestBody.setDescription('A custom permission grant policy to customize conditions for granting consent.');



result = await client.policies().permissionGrantPolicies().post(requestBody);


```