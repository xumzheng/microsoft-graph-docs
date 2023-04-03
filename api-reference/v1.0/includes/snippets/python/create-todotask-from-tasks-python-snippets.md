---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TodoTask();
requestBody.setTitle('A new task');

requestBody.setCategories(['Important', ]);

linkedResourcesLinkedResource1 = LinkedResource();
linkedResourcesLinkedResource1.setWebUrl('http://microsoft.com');

linkedResourcesLinkedResource1.setApplicationName('Microsoft');

linkedResourcesLinkedResource1.setDisplayName('Microsoft');


linkedResourcesArray []= linkedResourcesLinkedResource1;
requestBody.setLinkedResources(linkedResourcesArray);




result = await client.me().todo().listsById('todoTaskList-id').tasks().post(requestBody);


```