---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CrossTenantAccessPolicy();
requestBody.setAllowedCloudEndpoints(['microsoftonline.us', 'partner.microsoftonline.cn', ]);



result = awaitclient.policies().crossTenantAccessPolicy().patch(requestBody);


```