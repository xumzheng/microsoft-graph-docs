---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingAppointment()
request_body.set@odatatype('#microsoft.graph.bookingAppointment')

end = DateTimeTimeZone()
end.set@odatatype('#microsoft.graph.dateTimeTimeZone')

end.setDateTime('2018-05-06T12:30:00.0000000+00:00')

end.setTimeZone('UTC')


request_body.setEnd($end)
invoiceDate = DateTimeTimeZone()
invoiceDate.set@odatatype('#microsoft.graph.dateTimeTimeZone')

invoiceDate.setDateTime('2018-05-06T12:30:00.0000000+00:00')

invoiceDate.setTimeZone('UTC')


request_body.setInvoiceDate($invoiceDate)
start = DateTimeTimeZone()
start.set@odatatype('#microsoft.graph.dateTimeTimeZone')

start.setDateTime('2018-05-06T12:00:00.0000000+00:00')

start.setTimeZone('UTC')


request_body.setStart($start)


result = await client.bookingBusinessesby_id('bookingBusiness-id').appointmentsby_id('bookingAppointment-id').patch(request_body)


```