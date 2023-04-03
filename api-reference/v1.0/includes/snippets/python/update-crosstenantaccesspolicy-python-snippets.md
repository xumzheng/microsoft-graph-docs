---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CrossTenantAccessPolicy();
requestBody.setAllowedCloudEndpoints(['microsoftonline.us', ]);



requestResult = graphServiceClient.policies().crossTenantAccessPolicy().patch(requestBody);


```