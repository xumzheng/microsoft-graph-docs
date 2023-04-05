---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LinkedResource()
request_body.set@odatatype('#microsoft.graph.linkedResource')

request_body.setWebUrl('http://microsoft.com')

request_body.setApplicationName('Microsoft')

request_body.setDisplayName('Microsoft')



result = await client.me.todo.lists._by_id('todoTaskList-id').tasks._by_id('todoTask-id').linkedResources._by_id('linkedResource-id').patch(request_body)


```