---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Permission();
requestBody.setRoles(['read', ]);



result = awaitclient.sitesById('site-id').permissionsById('permission-id').patch(requestBody);


```