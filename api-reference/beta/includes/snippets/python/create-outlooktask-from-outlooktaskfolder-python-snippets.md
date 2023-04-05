---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTask()
request_body.setSubject('Shop for dinner')

startDateTime = DateTimeTimeZone()
startDateTime.setDateTime('2016-04-23T18:00:00')

startDateTime.setTimeZone('Pacific Standard Time')


request_body.setStartDateTime($startDateTime)
dueDateTime = DateTimeTimeZone()
dueDateTime.setDateTime('2016-04-25T13:00:00')

dueDateTime.setTimeZone('Pacific Standard Time')


request_body.setDueDateTime($dueDateTime)


result = await client.me.outlook.taskFolders_by_id('outlookTaskFolder-id').tasks.post(request_body)


```