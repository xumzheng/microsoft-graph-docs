---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Event();
requestBody.setSubject('Prep for customer meeting');

body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('Does this time work for you?');


requestBody.setBody($body);
start = DateTimeTimeZone();
start.setDateTime('2019-11-20T13:00:00');

start.setTimeZone('Pacific Standard Time');


requestBody.setStart($start);
end = DateTimeTimeZone();
end.setDateTime('2019-11-20T14:00:00');

end.setTimeZone('Pacific Standard Time');


requestBody.setEnd($end);
location = Location();
location.setDisplayName('Cordova conference room');


requestBody.setLocation($location);
attendeesAttendee1 = Attendee();
attendeesAttendee1EmailAddress = EmailAddress();
attendeesAttendee1EmailAddress.setAddress('AdeleV@contoso.OnMicrosoft.com');

attendeesAttendee1EmailAddress.setName('Adele Vance');


attendeesAttendee1.setEmailAddress($attendeesAttendee1EmailAddress);
attendeesAttendee1.setType(AttendeeType('required'));


attendeesArray []= attendeesAttendee1;
requestBody.setAttendees(attendeesArray);


requestBody.setAllowNewTimeProposals(true);

requestBody.setIsOnlineMeeting(true);

requestBody.setOnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'));


request_config = EventsRequestBuilderPostRequestConfiguration();

headers = [
'Prefer' => 'outlook.timezone="Pacific Standard Time"',
];

request_config.headers = headers;


result = await client.me().events().post(requestBody, request_config);


```