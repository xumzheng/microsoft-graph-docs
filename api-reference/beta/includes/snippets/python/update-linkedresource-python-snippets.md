---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LinkedResource()
request_body.@odatatype = '#microsoft.graph.linkedResource'

request_body.webUrl = 'http://microsoft.com'

request_body.applicationName = 'Microsoft'

request_body.displayName = 'Microsoft'



request_configuration = LinkedResourceRequestBuilderPatchRequestConfiguration(
)


result = await client.me.todo.lists_by_id('todoTaskList-id').tasks_by_id('todoTask-id').linkedResources_by_id('linkedResource-id').patch(request_body = request_body)


```