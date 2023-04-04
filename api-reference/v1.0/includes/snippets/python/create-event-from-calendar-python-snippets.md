---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Event();
request_body.setSubject('Let\'s go for lunch');

body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('Does mid month work for you?');


request_body.setBody($body);
start = DateTimeTimeZone();
start.setDateTime('2019-03-15T12:00:00');

start.setTimeZone('Pacific Standard Time');


request_body.setStart($start);
end = DateTimeTimeZone();
end.setDateTime('2019-03-15T14:00:00');

end.setTimeZone('Pacific Standard Time');


request_body.setEnd($end);
location = Location();
location.setDisplayName('Harry\'s Bar');


request_body.setLocation($location);
attendeesAttendee1 = Attendee();
attendeesAttendee1EmailAddress = EmailAddress();
attendeesAttendee1EmailAddress.setAddress('adelev@contoso.onmicrosoft.com');

attendeesAttendee1EmailAddress.setName('Adele Vance');


attendeesAttendee1.setEmailAddress($attendeesAttendee1EmailAddress);
attendeesAttendee1.setType(AttendeeType('required'));


attendeesArray []= attendeesAttendee1;
request_body.setAttendees(attendeesArray);


request_body.setTransactionId('7E163156-7762-4BEB-A1C6-729EA81755A7');



result = await client.me.calendarsById('calendar-id').events.post(request_body);


```