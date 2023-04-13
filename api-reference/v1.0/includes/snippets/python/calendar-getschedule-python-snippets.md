---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetSchedulePostRequestBody()
request_body.Schedules(['adelev@contoso.onmicrosoft.com', 'meganb@contoso.onmicrosoft.com', ])

start_time = DateTimeTimeZone()
startTime.dateTime = '2019-03-15T09:00:00'

startTime.timeZone = 'Pacific Standard Time'


request_body.start_time = startTime
end_time = DateTimeTimeZone()
endTime.dateTime = '2019-03-15T18:00:00'

endTime.timeZone = 'Pacific Standard Time'


request_body.end_time = endTime
request_body.availability_view_interval = 60



request_configuration = GetScheduleRequestBuilder.GetScheduleRequestBuilderPostRequestConfiguration(
headers = {
	'Prefer' : "outlook.timezone=\"Pacific Standard Time\"",
}

)


result = await client.me.calendar.getSchedule.post(request_body = request_body, request_configuration = request_configuration)


```