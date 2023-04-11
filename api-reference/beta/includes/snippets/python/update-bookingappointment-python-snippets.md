---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingAppointment()
request_body.@odatatype = '#microsoft.graph.bookingAppointment'

end = DateTimeTimeZone()
end.@odatatype = '#microsoft.graph.dateTimeTimeZone'

end.dateTime = '2018-05-06T12:30:00.0000000+00:00'

end.timeZone = 'UTC'


request_body.end = end
invoiceDate = DateTimeTimeZone()
invoiceDate.@odatatype = '#microsoft.graph.dateTimeTimeZone'

invoiceDate.dateTime = '2018-05-06T12:30:00.0000000+00:00'

invoiceDate.timeZone = 'UTC'


request_body.invoiceDate = invoiceDate
start = DateTimeTimeZone()
start.@odatatype = '#microsoft.graph.dateTimeTimeZone'

start.dateTime = '2018-05-06T12:00:00.0000000+00:00'

start.timeZone = 'UTC'


request_body.start = start


request_configuration = BookingAppointmentRequestBuilderPatchRequestConfiguration(
)


result = await client.bookingBusinesses_by_id('bookingBusiness-id').appointments_by_id('bookingAppointment-id').patch(request_body = request_body)


```