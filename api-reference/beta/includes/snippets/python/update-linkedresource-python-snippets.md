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



result = await client.me.todo.listsby_id('todoTaskList-id').tasksby_id('todoTask-id').linkedResourcesby_id('linkedResource-id').patch(request_body)


```