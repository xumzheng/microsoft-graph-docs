---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
request_body.setSubject('Let\'s go for lunch')

body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('Does noon work for you?')


request_body.setBody($body)
start = DateTimeTimeZone()
start.setDateTime('2017-04-15T12:00:00')

start.setTimeZone('Pacific Standard Time')


request_body.setStart($start)
end = DateTimeTimeZone()
end.setDateTime('2017-04-15T14:00:00')

end.setTimeZone('Pacific Standard Time')


request_body.setEnd($end)
location = Location()
location.setDisplayName('Harry\'s Bar')


request_body.setLocation($location)
attendeesAttendee1 = Attendee()
attendeesAttendee1EmailAddress = EmailAddress()
attendeesAttendee1EmailAddress.setAddress('samanthab@contoso.onmicrosoft.com')

attendeesAttendee1EmailAddress.setName('Samantha Booth')


attendeesAttendee1.setEmailAddress($attendeesAttendee1EmailAddress)
attendeesAttendee1.setType(AttendeeType('required'))


attendeesArray []= attendeesAttendee1;
request_body.setAttendees(attendeesArray)


request_body.setAllowNewTimeProposals(true)

request_body.setIsOnlineMeeting(true)

request_body.setOnlineMeetingProvider(OnlineMeetingProviderType('teamsforbusiness'))


request_config = EventsRequestBuilderPostRequestConfiguration(
request_config = EventsRequestBuilderPostRequestConfiguration(query_params=)
headers['Prefer'] = "outlook.timezone=\"Pacific Standard Time\""


result = await client.me.events.post(request_body, request_config, headers=request_config)


```