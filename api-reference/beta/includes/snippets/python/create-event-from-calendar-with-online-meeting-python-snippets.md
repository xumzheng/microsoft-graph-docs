---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
request_body.subject = 'Let\'s go for lunch'

body = ItemBody()
body.ContentType(BodyType('html'))

body.content = 'Does next month work for you?'


request_body.body = body
start = DateTimeTimeZone()
start.dateTime = '2019-03-10T12:00:00'

start.timeZone = 'Pacific Standard Time'


request_body.start = start
end = DateTimeTimeZone()
end.dateTime = '2019-03-10T14:00:00'

end.timeZone = 'Pacific Standard Time'


request_body.end = end
location = Location()
location.displayName = 'Harry\'s Bar'


request_body.location = location
attendeesAttendee1 = Attendee()
attendeesAttendee1EmailAddress = EmailAddress()
attendeesAttendee1EmailAddress.address = 'adelev@contoso.onmicrosoft.com'

attendeesAttendee1EmailAddress.name = 'Adele Vance'


attendeesAttendee1.emailAddress = attendeesAttendee1EmailAddress
attendeesAttendee1.Type(AttendeeType('required'))


attendeesArray []= attendeesAttendee1;
request_body.attendees(attendeesArray)


request_body.isOnlineMeeting = true

request_body.OnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'))



request_configuration = EventsRequestBuilderPostRequestConfiguration(
)


result = await client.me.calendars_by_id('calendar-id').events.post(request_body = request_body)


```