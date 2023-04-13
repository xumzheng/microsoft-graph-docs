---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingAppointment()
request_body.@odatatype = '#microsoft.graph.bookingAppointment'

end_date_time = DateTimeTimeZone()
endDateTime.@odatatype = '#microsoft.graph.dateTimeTimeZone'

endDateTime.dateTime = '2018-05-06T12:30:00.0000000+00:00'

endDateTime.timeZone = 'UTC'


request_body.end_date_time = endDateTime
start_date_time = DateTimeTimeZone()
startDateTime.@odatatype = '#microsoft.graph.dateTimeTimeZone'

startDateTime.dateTime = '2018-05-06T12:00:00.0000000+00:00'

startDateTime.timeZone = 'UTC'


request_body.start_date_time = startDateTime



result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').appointments_by_id('bookingAppointment-id').patch(request_body = request_body)


```