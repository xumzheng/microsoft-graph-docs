---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TodoTask()
request_body.setTitle('A new task')

request_body.setCategories(['Important', ])

linkedResourcesLinkedResource1 = LinkedResource()
linkedResourcesLinkedResource1.setWebUrl('http://microsoft.com')

linkedResourcesLinkedResource1.setApplicationName('Microsoft')

linkedResourcesLinkedResource1.setDisplayName('Microsoft')


linkedResourcesArray []= linkedResourcesLinkedResource1;
request_body.setLinkedResources(linkedResourcesArray)




result = await client.me.todo.lists._by_id('todoTaskList-id').tasks.post(request_body)


```