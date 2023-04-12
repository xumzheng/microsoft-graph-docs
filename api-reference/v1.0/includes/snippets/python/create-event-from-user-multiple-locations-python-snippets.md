---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Event()
request_body.subject = 'Plan summer company picnic'

body = ItemBody()
body.ContentType(BodyType('html'))

body.content = 'Let\'s kick-start this event planning!'


request_body.body = body
start = DateTimeTimeZone()
start.dateTime = '2017-08-30T11:00:00'

start.timeZone = 'Pacific Standard Time'


request_body.start = start
end = DateTimeTimeZone()
end.dateTime = '2017-08-30T12:00:00'

end.timeZone = 'Pacific Standard Time'


request_body.end = end
attendeesAttendee1 = Attendee()
attendeesAttendee1EmailAddress = EmailAddress()
attendeesAttendee1EmailAddress.address = 'DanaS@contoso.onmicrosoft.com'

attendeesAttendee1EmailAddress.name = 'Dana Swope'


attendeesAttendee1.emailAddress = attendeesAttendee1EmailAddress
attendeesAttendee1.Type(AttendeeType('required'))


attendeesArray []= attendeesAttendee1;
attendeesAttendee2 = Attendee()
attendeesAttendee2EmailAddress = EmailAddress()
attendeesAttendee2EmailAddress.address = 'AlexW@contoso.onmicrosoft.com'

attendeesAttendee2EmailAddress.name = 'Alex Wilber'


attendeesAttendee2.emailAddress = attendeesAttendee2EmailAddress
attendeesAttendee2.Type(AttendeeType('required'))


attendeesArray []= attendeesAttendee2;
request_body.attendees(attendeesArray)


location = Location()
location.displayName = 'Conf Room 3; Fourth Coffee; Home Office'

location.LocationType(LocationType('default'))


request_body.location = location
locationsLocation1 = Location()
locationsLocation1.displayName = 'Conf Room 3'


locationsArray []= locationsLocation1;
locationsLocation2 = Location()
locationsLocation2.displayName = 'Fourth Coffee'

locationsLocation2Address = PhysicalAddress()
locationsLocation2Address.street = '4567 Main St'

locationsLocation2Address.city = 'Redmond'

locationsLocation2Address.state = 'WA'

locationsLocation2Address.countryOrRegion = 'US'

locationsLocation2Address.postalCode = '32008'


locationsLocation2.address = locationsLocation2Address
locationsLocation2Coordinates = OutlookGeoCoordinates()
locationsLocation2Coordinates.latitude = 47.672

locationsLocation2Coordinates.longitude = -102.103


locationsLocation2.coordinates = locationsLocation2Coordinates

locationsArray []= locationsLocation2;
locationsLocation3 = Location()
locationsLocation3.displayName = 'Home Office'


locationsArray []= locationsLocation3;
request_body.locations(locationsArray)


request_body.allowNewTimeProposals = true


headers = {
'Prefer' : "outlook.timezone=\"Pacific Standard Time\"",
}

)


result = await client.me.events.post(request_body = request_body, request_configuration = request_configuration)


```