---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BookingAppointment();
requestBody.set@odatatype('#microsoft.graph.bookingAppointment');

end = DateTimeTimeZone();
end.set@odatatype('#microsoft.graph.dateTimeTimeZone');

end.setDateTime('2018-05-06T12:30:00.0000000+00:00');

end.setTimeZone('UTC');


requestBody.setEnd($end);
invoiceDate = DateTimeTimeZone();
invoiceDate.set@odatatype('#microsoft.graph.dateTimeTimeZone');

invoiceDate.setDateTime('2018-05-06T12:30:00.0000000+00:00');

invoiceDate.setTimeZone('UTC');


requestBody.setInvoiceDate($invoiceDate);
start = DateTimeTimeZone();
start.set@odatatype('#microsoft.graph.dateTimeTimeZone');

start.setDateTime('2018-05-06T12:00:00.0000000+00:00');

start.setTimeZone('UTC');


requestBody.setStart($start);


result = awaitclient.bookingBusinessesById('bookingBusiness-id').appointmentsById('bookingAppointment-id').patch(requestBody);


```