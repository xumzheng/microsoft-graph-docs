---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = LinkedResource();
requestBody.setWebUrl('https://microsoft.com');

requestBody.setApplicationName('Microsoft');

requestBody.setDisplayName('Microsoft');

requestBody.setExternalId('dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9');



result = await client.me().todo().listsById('todoTaskList-id').tasksById('todoTask-id').linkedResources().post(requestBody);


```