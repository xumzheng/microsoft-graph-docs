---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ShiftPreferences();
request_body.setId('SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7');

availabilityShiftAvailability1 = ShiftAvailability();
availabilityShiftAvailability1Recurrence = PatternedRecurrence();
availabilityShiftAvailability1RecurrencePattern = RecurrencePattern();
availabilityShiftAvailability1RecurrencePattern.setType(RecurrencePatternType('weekly'));

availabilityShiftAvailability1RecurrencePattern.setDaysOfWeek([availabilityShiftAvailability1RecurrencePattern.setDayOfWeek(DayOfWeek('monday'));
availabilityShiftAvailability1RecurrencePattern.setDayOfWeek(DayOfWeek('wednesday'));
availabilityShiftAvailability1RecurrencePattern.setDayOfWeek(DayOfWeek('friday'));
]);

availabilityShiftAvailability1RecurrencePattern.setInterval(1);


availabilityShiftAvailability1Recurrence.setPattern($availabilityShiftAvailability1RecurrencePattern);
availabilityShiftAvailability1RecurrenceRange = RecurrenceRange();
availabilityShiftAvailability1RecurrenceRange.setType(RecurrenceRangeType('noend'));


availabilityShiftAvailability1Recurrence.setRange($availabilityShiftAvailability1RecurrenceRange);

availabilityShiftAvailability1.setRecurrence($availabilityShiftAvailability1Recurrence);
availabilityShiftAvailability1.setTimeZone('Pacific Standard Time');

availabilityShiftAvailability1.setTimeSlots(null);


availabilityArray []= availabilityShiftAvailability1;
request_body.setAvailability(availabilityArray);


additionalData = [
'@odata.etag' => '1a371e53-f0a6-4327-a1ee-e3c56e4b38aa', 
];
request_body.setAdditionalData(additionalData);




result = await client.usersById('user-id').settings.shiftPreferences.patch(request_body);


```