---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FindMeetingTimesPostRequestBody()
attendeesAttendeeBase1 = AttendeeBase()
attendeesAttendeeBase1.Type(AttendeeType('required'))

attendeesAttendeeBase1EmailAddress = EmailAddress()
attendeesAttendeeBase1EmailAddress.name = 'Alex Wilbur'

attendeesAttendeeBase1EmailAddress.address = 'alexw@contoso.onmicrosoft.com'


attendeesAttendeeBase1.emailAddress = attendeesAttendeeBase1EmailAddress

attendeesArray []= attendeesAttendeeBase1;
request_body.attendees(attendeesArray)


locationConstraint = LocationConstraint()
locationConstraint.isRequired = false

locationConstraint.suggestLocation = false

locationsLocationConstraintItem1 = LocationConstraintItem()
locationsLocationConstraintItem1.resolveAvailability = false

locationsLocationConstraintItem1.displayName = 'Conf room Hood'


locationsArray []= locationsLocationConstraintItem1;
locationConstraint.locations(locationsArray)



request_body.locationConstraint = locationConstraint
timeConstraint = TimeConstraint()
timeConstraint.ActivityDomain(ActivityDomain('work'))

timeSlotsTimeSlot1 = TimeSlot()
timeSlotsTimeSlot1Start = DateTimeTimeZone()
timeSlotsTimeSlot1Start.dateTime = '2019-04-16T09:00:00'

timeSlotsTimeSlot1Start.timeZone = 'Pacific Standard Time'


timeSlotsTimeSlot1.start = timeSlotsTimeSlot1Start
timeSlotsTimeSlot1End = DateTimeTimeZone()
timeSlotsTimeSlot1End.dateTime = '2019-04-18T17:00:00'

timeSlotsTimeSlot1End.timeZone = 'Pacific Standard Time'


timeSlotsTimeSlot1.end = timeSlotsTimeSlot1End

timeSlotsArray []= timeSlotsTimeSlot1;
timeConstraint.timeslots(timeSlotsArray)



request_body.timeConstraint = timeConstraint
request_body.isOrganizerOptional = false

request_body.meetingduration =  \DateInterval('PT1H')

request_body.returnSuggestionReasons = true

request_body.minimumAttendeePercentage = '100'



request_configuration = FindMeetingTimesRequestBuilderPostRequestConfiguration(
headers = {
		'Prefer' : "outlook.timezone=\"Pacific Standard Time\"",
}

)


result = await client.me.findMeetingTimes.post(request_body = request_body, request_configuration = request_configuration)


```