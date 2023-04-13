---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingAppointment()
request_body.@odatatype = '#microsoft.graph.bookingAppointment'

endDateTime = DateTimeTimeZone()
endDateTime.@odatatype = '#microsoft.graph.dateTimeTimeZone'

endDateTime.dateTime = '2018-05-06T12:30:00.0000000+00:00'

endDateTime.timeZone = 'UTC'


request_body.endDateTime = endDateTime
startDateTime = DateTimeTimeZone()
startDateTime.@odatatype = '#microsoft.graph.dateTimeTimeZone'

startDateTime.dateTime = '2018-05-06T12:00:00.0000000+00:00'

startDateTime.timeZone = 'UTC'


request_body.startDateTime = startDateTime



result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').appointments_by_id('bookingAppointment-id').patch(request_body = request_body)


```