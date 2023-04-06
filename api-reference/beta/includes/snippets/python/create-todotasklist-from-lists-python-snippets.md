---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TodoTaskList()
request_body.setDisplayName('Travel items')



result = await client.me.todo.lists.post(request_body)


```