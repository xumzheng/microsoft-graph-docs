---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetSchedulePostRequestBody()
request_body.Schedules(['adelev@contoso.onmicrosoft.com', 'meganb@contoso.onmicrosoft.com', ])

startTime = DateTimeTimeZone()
startTime.dateTime = '2019-03-15T09:00:00'

startTime.timeZone = 'Pacific Standard Time'


request_body.startTime = startTime
endTime = DateTimeTimeZone()
endTime.dateTime = '2019-03-15T18:00:00'

endTime.timeZone = 'Pacific Standard Time'


request_body.endTime = endTime
request_body.availabilityViewInterval = 60


headers = {
'Prefer' : "outlook.timezone=\"Pacific Standard Time\"",
}

)


result = await client.me.calendar.getSchedule.post(request_body = request_body, request_configuration = request_configuration)


```