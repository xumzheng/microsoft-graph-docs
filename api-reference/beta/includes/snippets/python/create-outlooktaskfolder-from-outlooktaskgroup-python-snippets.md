---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTaskFolder()
request_body.setName('Cooking')



result = await client.me.outlook.taskGroupsby_id('outlookTaskGroup-id').taskFolders.post(request_body)


```