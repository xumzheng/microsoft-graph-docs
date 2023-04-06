---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TodoTaskList()
request_body.setDisplayName('Vacation Plan')


request_config = TodoTaskListRequestBuilderPatchRequestConfiguration(
request_config = TodoTaskListRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.todo.lists_by_id('todoTaskList-id').patch(request_body, headers=)


```