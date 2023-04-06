---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LinkedResource()
request_body.setWebUrl('https://microsoft.com')

request_body.setApplicationName('Microsoft')

request_body.setDisplayName('Microsoft')

request_body.setExternalId('dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9')


request_config = LinkedResourcesRequestBuilderPostRequestConfiguration(
request_config = LinkedResourcesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.todo.lists_by_id('todoTaskList-id').tasks_by_id('todoTask-id').linkedResources.post(request_body, headers=)


```