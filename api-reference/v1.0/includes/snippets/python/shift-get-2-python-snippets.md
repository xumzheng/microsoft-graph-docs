---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ShiftPreferences()
request_body.id = 'SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7'

availabilityShiftAvailability1 = ShiftAvailability()
availabilityShiftAvailability1Recurrence = PatternedRecurrence()
availabilityShiftAvailability1RecurrencePattern = RecurrencePattern()
availabilityShiftAvailability1RecurrencePattern.Type(RecurrencePatternType('weekly'))

availabilityShiftAvailability1RecurrencePattern.DaysOfWeek([availabilityShiftAvailability1RecurrencePattern.DayOfWeek(DayOfWeek('monday'))
availabilityShiftAvailability1RecurrencePattern.DayOfWeek(DayOfWeek('wednesday'))
availabilityShiftAvailability1RecurrencePattern.DayOfWeek(DayOfWeek('friday'))
])

availabilityShiftAvailability1RecurrencePattern.interval = 1


availabilityShiftAvailability1Recurrence.pattern = availabilityShiftAvailability1RecurrencePattern
availabilityShiftAvailability1RecurrenceRange = RecurrenceRange()
availabilityShiftAvailability1RecurrenceRange.Type(RecurrenceRangeType('noend'))


availabilityShiftAvailability1Recurrence.range = availabilityShiftAvailability1RecurrenceRange

availabilityShiftAvailability1.recurrence = availabilityShiftAvailability1Recurrence
availabilityShiftAvailability1.timeZone = 'Pacific Standard Time'

availabilityShiftAvailability1.timeSlots=null


availabilityArray []= availabilityShiftAvailability1;
request_body.availability(availabilityArray)


additionalData = [
'@odata.etag' => '1a371e53-f0a6-4327-a1ee-e3c56e4b38aa', 
];
request_body.additionaldata(additionalData)





result = await client.users_by_id('user-id').settings.shiftPreferences.patch(request_body = request_body)


```