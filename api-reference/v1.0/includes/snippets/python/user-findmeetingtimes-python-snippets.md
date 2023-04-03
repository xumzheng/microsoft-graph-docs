---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = FindMeetingTimesPostRequestBody();
attendeesAttendeeBase1 = AttendeeBase();
attendeesAttendeeBase1.setType(AttendeeType('required'));

attendeesAttendeeBase1EmailAddress = EmailAddress();
attendeesAttendeeBase1EmailAddress.setName('Alex Wilbur');

attendeesAttendeeBase1EmailAddress.setAddress('alexw@contoso.onmicrosoft.com');


attendeesAttendeeBase1.setEmailAddress($attendeesAttendeeBase1EmailAddress);

attendeesArray []= attendeesAttendeeBase1;
requestBody.setAttendees(attendeesArray);


locationConstraint = LocationConstraint();
locationConstraint.setIsRequired(false);

locationConstraint.setSuggestLocation(false);

locationsLocationConstraintItem1 = LocationConstraintItem();
locationsLocationConstraintItem1.setResolveAvailability(false);

locationsLocationConstraintItem1.setDisplayName('Conf room Hood');


locationsArray []= locationsLocationConstraintItem1;
locationConstraint.setLocations(locationsArray);



requestBody.setLocationConstraint($locationConstraint);
timeConstraint = TimeConstraint();
timeConstraint.setActivityDomain(ActivityDomain('work'));

timeSlotsTimeSlot1 = TimeSlot();
timeSlotsTimeSlot1Start = DateTimeTimeZone();
timeSlotsTimeSlot1Start.setDateTime('2019-04-16T09:00:00');

timeSlotsTimeSlot1Start.setTimeZone('Pacific Standard Time');


timeSlotsTimeSlot1.setStart($timeSlotsTimeSlot1Start);
timeSlotsTimeSlot1End = DateTimeTimeZone();
timeSlotsTimeSlot1End.setDateTime('2019-04-18T17:00:00');

timeSlotsTimeSlot1End.setTimeZone('Pacific Standard Time');


timeSlotsTimeSlot1.setEnd($timeSlotsTimeSlot1End);

timeSlotsArray []= timeSlotsTimeSlot1;
timeConstraint.setTimeSlots(timeSlotsArray);



requestBody.setTimeConstraint($timeConstraint);
requestBody.setIsOrganizerOptional(false);

$requestBody.setMeetingDuration( \DateInterval('PT1H'));

requestBody.setReturnSuggestionReasons(true);

requestBody.setMinimumAttendeePercentage('100');


requestConfiguration = FindMeetingTimesRequestBuilderPostRequestConfiguration();

headers = [
'Prefer' => 'outlook.timezone="Pacific Standard Time"',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().findMeetingTimes().post(requestBody, requestConfiguration);


```