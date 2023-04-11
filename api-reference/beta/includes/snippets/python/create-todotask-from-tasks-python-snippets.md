---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TodoTask()
request_body.title = 'A new task'

request_body.Categories(['Important', ])

linkedResourcesLinkedResource1 = LinkedResource()
linkedResourcesLinkedResource1.webUrl = 'http://microsoft.com'

linkedResourcesLinkedResource1.applicationName = 'Microsoft'

linkedResourcesLinkedResource1.displayName = 'Microsoft'


linkedResourcesArray []= linkedResourcesLinkedResource1;
request_body.linkedresources(linkedResourcesArray)




request_configuration = TasksRequestBuilderPostRequestConfiguration(
)


result = await client.me.todo.lists_by_id('todoTaskList-id').tasks.post(request_body = request_body)


```