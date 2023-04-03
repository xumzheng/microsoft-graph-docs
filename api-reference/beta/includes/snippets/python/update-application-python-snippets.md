---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Application();
requestBody.setDisplayName('New display name');



result = await client.applicationsById('application-id').patch(requestBody);


```