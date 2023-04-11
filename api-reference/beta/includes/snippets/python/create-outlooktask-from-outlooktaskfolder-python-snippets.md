---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTask()
request_body.subject = 'Shop for dinner'

startDateTime = DateTimeTimeZone()
startDateTime.dateTime = '2016-04-23T18:00:00'

startDateTime.timeZone = 'Pacific Standard Time'


request_body.startDateTime = startDateTime
dueDateTime = DateTimeTimeZone()
dueDateTime.dateTime = '2016-04-25T13:00:00'

dueDateTime.timeZone = 'Pacific Standard Time'


request_body.dueDateTime = dueDateTime



result = await client.me.outlook.taskFolders_by_id('outlookTaskFolder-id').tasks.post(request_body = request_body)


```