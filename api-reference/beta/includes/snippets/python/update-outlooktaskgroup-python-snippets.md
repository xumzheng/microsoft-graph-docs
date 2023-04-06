---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTaskGroup()
request_body.setName('Personal Tasks')



result = await client.me.outlook.taskGroups_by_id('outlookTaskGroup-id').patch(request_body, headers=)


```