---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FindMeetingTimesPostRequestBody()
attendees_attendee_base1 = AttendeeBase()
attendeesAttendeeBase1.Type(AttendeeType('required'))

attendees_attendee_base1_email_address = EmailAddress()
attendeesAttendeeBase1EmailAddress.name = 'Alex Wilbur'

attendeesAttendeeBase1EmailAddress.address = 'alexw@contoso.onmicrosoft.com'


attendeesAttendeeBase1.email_address = attendeesAttendeeBase1EmailAddress

attendeesArray []= attendeesAttendeeBase1;
request_body.attendees(attendeesArray)


location_constraint = LocationConstraint()
locationConstraint.is_required = False

locationConstraint.suggest_location = False

locations_location_constraint_item1 = LocationConstraintItem()
locationsLocationConstraintItem1.resolve_availability = False

locationsLocationConstraintItem1.displayName = 'Conf room Hood'


locationsArray []= locationsLocationConstraintItem1;
locationConstraint.locations(locationsArray)



request_body.location_constraint = locationConstraint
time_constraint = TimeConstraint()
timeConstraint.ActivityDomain(ActivityDomain('work'))

time_slots_time_slot1 = TimeSlot()
time_slots_time_slot1_start = DateTimeTimeZone()
timeSlotsTimeSlot1Start.dateTime = '2019-04-16T09:00:00'

timeSlotsTimeSlot1Start.timeZone = 'Pacific Standard Time'


timeSlotsTimeSlot1.start = timeSlotsTimeSlot1Start
time_slots_time_slot1_end = DateTimeTimeZone()
timeSlotsTimeSlot1End.dateTime = '2019-04-18T17:00:00'

timeSlotsTimeSlot1End.timeZone = 'Pacific Standard Time'


timeSlotsTimeSlot1.end = timeSlotsTimeSlot1End

timeSlotsArray []= timeSlotsTimeSlot1;
timeConstraint.timeslots(timeSlotsArray)



request_body.time_constraint = timeConstraint
request_body.is_organizer_optional = False

request_body.meetingduration =  \DateInterval('PT1H')

request_body.return_suggestion_reasons = True

request_body.minimumAttendeePercentage = '100'



request_configuration = FindMeetingTimesRequestBuilder.FindMeetingTimesRequestBuilderPostRequestConfiguration(
headers = {
'Prefer' : "outlook.timezone=\"Pacific Standard Time\"",
}

)


result = await client.me.findMeetingTimes.post(request_body = request_body, request_configuration = request_configuration)


```