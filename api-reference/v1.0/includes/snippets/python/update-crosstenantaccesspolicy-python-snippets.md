---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CrossTenantAccessPolicy();
requestBody.setAllowedCloudEndpoints(['microsoftonline.us', ]);



result = await client.policies().crossTenantAccessPolicy().patch(requestBody);


```