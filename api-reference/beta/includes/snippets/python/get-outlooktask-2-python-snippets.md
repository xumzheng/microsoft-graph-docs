---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OutlookTaskRequestBuilderGetRequestConfiguration()

headers = [
	'Prefer' => 'outlook.timezone="Pacific Standard Time"',
]

request_config.headers = headers


result = await client.me.outlook.tasksById('outlookTask-id').get(request_config)


```