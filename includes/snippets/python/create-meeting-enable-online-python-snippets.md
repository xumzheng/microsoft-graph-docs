---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
request_body.setSubject('Prep for customer meeting')

body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('Does this time work for you?')


request_body.setBody($body)
start = DateTimeTimeZone()
start.setDateTime('2019-11-20T13:00:00')

start.setTimeZone('Pacific Standard Time')


request_body.setStart($start)
end = DateTimeTimeZone()
end.setDateTime('2019-11-20T14:00:00')

end.setTimeZone('Pacific Standard Time')


request_body.setEnd($end)
location = Location()
location.setDisplayName('Cordova conference room')


request_body.setLocation($location)
attendeesAttendee1 = Attendee()
attendeesAttendee1EmailAddress = EmailAddress()
attendeesAttendee1EmailAddress.setAddress('AdeleV@contoso.OnMicrosoft.com')

attendeesAttendee1EmailAddress.setName('Adele Vance')


attendeesAttendee1.setEmailAddress($attendeesAttendee1EmailAddress)
attendeesAttendee1.setType(AttendeeType('required'))


attendeesArray []= attendeesAttendee1;
request_body.setAttendees(attendeesArray)


request_body.setAllowNewTimeProposals(true)

request_body.setIsOnlineMeeting(true)

request_body.setOnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'))


request_config = EventsRequestBuilderPostRequestConfiguration()

headers = [
'Prefer' => 'outlook.timezone="Pacific Standard Time"',
]

request_config.headers = headers


result = await client.me_events.post(request_body, request_config)


```