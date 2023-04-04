---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = LinkedResource();
request_body.setWebUrl('https://microsoft.com');

request_body.setApplicationName('Microsoft');

request_body.setDisplayName('Microsoft');

request_body.setExternalId('dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9');



result = await client.me.todo.listsById('todoTaskList-id').tasksById('todoTask-id').linkedResources.post(request_body);


```