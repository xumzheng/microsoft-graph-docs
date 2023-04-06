---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetSchedulePostRequestBody()
request_body.setSchedules(['adelev@contoso.onmicrosoft.com', 'meganb@contoso.onmicrosoft.com', ])

startTime = DateTimeTimeZone()
startTime.setDateTime('2019-03-15T09:00:00')

startTime.setTimeZone('Pacific Standard Time')


request_body.setStartTime($startTime)
endTime = DateTimeTimeZone()
endTime.setDateTime('2019-03-15T18:00:00')

endTime.setTimeZone('Pacific Standard Time')


request_body.setEndTime($endTime)
request_body.setAvailabilityViewInterval(60)


request_config = GetScheduleRequestBuilderPostRequestConfiguration(
request_config = GetScheduleRequestBuilderPostRequestConfiguration(query_params=)
headers['Prefer'] = "outlook.timezone=\"Pacific Standard Time\""


result = await client.me.calendar.getSchedule.post(request_body, request_config, headers=request_config)


```