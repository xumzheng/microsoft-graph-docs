---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = BookingAppointment();
request_body.set@odatatype('#microsoft.graph.bookingAppointment');

endDateTime = DateTimeTimeZone();
endDateTime.set@odatatype('#microsoft.graph.dateTimeTimeZone');

endDateTime.setDateTime('2018-05-06T12:30:00.0000000+00:00');

endDateTime.setTimeZone('UTC');


request_body.setEndDateTime($endDateTime);
startDateTime = DateTimeTimeZone();
startDateTime.set@odatatype('#microsoft.graph.dateTimeTimeZone');

startDateTime.setDateTime('2018-05-06T12:00:00.0000000+00:00');

startDateTime.setTimeZone('UTC');


request_body.setStartDateTime($startDateTime);


result = await client.solutions().bookingBusinessesById('bookingBusiness-id').appointmentsById('bookingAppointment-id').patch(request_body);


```