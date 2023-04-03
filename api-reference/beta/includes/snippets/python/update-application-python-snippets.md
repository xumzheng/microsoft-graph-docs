---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Application();
requestBody.setDisplayName('New display name');



result = awaitclient.applicationsById('application-id').patch(requestBody);


```