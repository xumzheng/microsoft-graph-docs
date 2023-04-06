---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OutlookTaskRequestBuilderGetRequestConfiguration(
request_config = OutlookTaskRequestBuilderGetRequestConfiguration(query_params=)
headers['Prefer'] = "outlook.timezone=\"Pacific Standard Time\""


result = await client.me.outlook.tasks_by_id('outlookTask-id').get(request_config, headers=request_config)


```