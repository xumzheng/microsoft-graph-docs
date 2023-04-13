---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTask()
request_body.subject = 'Shop for children\'s weekend'

start_date_time = DateTimeTimeZone()
startDateTime.dateTime = '2016-05-03T09:00:00'

startDateTime.timeZone = 'Eastern Standard Time'


request_body.start_date_time = startDateTime
due_date_time = DateTimeTimeZone()
dueDateTime.dateTime = '2016-05-05T16:00:00'

dueDateTime.timeZone = 'Eastern Standard Time'


request_body.due_date_time = dueDateTime


request_configuration = TasksRequestBuilder.TasksRequestBuilderPostRequestConfiguration(
headers = {
		'Prefer' : "outlook.timezone=\"Pacific Standard Time\"",
}

)


result = await client.me.outlook.tasks.post(request_body = request_body, request_configuration = request_configuration)


```