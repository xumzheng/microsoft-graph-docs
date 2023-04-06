---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FindMeetingTimesPostRequestBody()
attendeesAttendeeBase1 = AttendeeBase()
attendeesAttendeeBase1.setType(AttendeeType('required'))

attendeesAttendeeBase1EmailAddress = EmailAddress()
attendeesAttendeeBase1EmailAddress.setName('Alex Wilbur')

attendeesAttendeeBase1EmailAddress.setAddress('alexw@contoso.onmicrosoft.com')


attendeesAttendeeBase1.setEmailAddress($attendeesAttendeeBase1EmailAddress)

attendeesArray []= attendeesAttendeeBase1;
request_body.setAttendees(attendeesArray)


locationConstraint = LocationConstraint()
locationConstraint.setIsRequired(false)

locationConstraint.setSuggestLocation(false)

locationsLocationConstraintItem1 = LocationConstraintItem()
locationsLocationConstraintItem1.setResolveAvailability(false)

locationsLocationConstraintItem1.setDisplayName('Conf room Hood')


locationsArray []= locationsLocationConstraintItem1;
locationConstraint.setLocations(locationsArray)



request_body.setLocationConstraint($locationConstraint)
timeConstraint = TimeConstraint()
timeConstraint.setActivityDomain(ActivityDomain('work'))

timeSlotsTimeSlot1 = TimeSlot()
timeSlotsTimeSlot1Start = DateTimeTimeZone()
timeSlotsTimeSlot1Start.setDateTime('2019-04-16T09:00:00')

timeSlotsTimeSlot1Start.setTimeZone('Pacific Standard Time')


timeSlotsTimeSlot1.setStart($timeSlotsTimeSlot1Start)
timeSlotsTimeSlot1End = DateTimeTimeZone()
timeSlotsTimeSlot1End.setDateTime('2019-04-18T17:00:00')

timeSlotsTimeSlot1End.setTimeZone('Pacific Standard Time')


timeSlotsTimeSlot1.setEnd($timeSlotsTimeSlot1End)

timeSlotsArray []= timeSlotsTimeSlot1;
timeConstraint.setTimeSlots(timeSlotsArray)



request_body.setTimeConstraint($timeConstraint)
request_body.setIsOrganizerOptional(false)

$request_body.setMeetingDuration( \DateInterval('PT1H'))

request_body.setReturnSuggestionReasons(true)

request_body.setMinimumAttendeePercentage('100')


request_config = FindMeetingTimesRequestBuilderPostRequestConfiguration(
request_config = FindMeetingTimesRequestBuilderPostRequestConfiguration(query_params=)
headers['Prefer'] = "outlook.timezone=\"Pacific Standard Time\""


result = await client.me.findMeetingTimes.post(request_body, request_config, headers=request_config)


```