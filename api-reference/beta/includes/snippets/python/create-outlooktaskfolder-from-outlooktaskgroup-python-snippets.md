---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTaskFolder()
request_body.setName('Cooking')



result = await client.me.outlook.taskGroups_by_id('outlookTaskGroup-id').taskFolders.post(request_body, headers=)


```