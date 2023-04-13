---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTask()
due_date_time = DateTimeTimeZone()
dueDateTime.dateTime = '2016-05-06T16:00:00'

dueDateTime.timeZone = 'Eastern Standard Time'


request_body.due_date_time = dueDateTime


request_configuration = OutlookTaskRequestBuilder.OutlookTaskRequestBuilderPatchRequestConfiguration(
headers = {
		'Prefer' : "outlook.timezone=\"Eastern Standard Time\"",
}

)


result = await client.me.outlook.tasks_by_id('outlookTask-id').patch(request_body = request_body, request_configuration = request_configuration)


```