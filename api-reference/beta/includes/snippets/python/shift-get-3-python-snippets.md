---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ShiftPreferencesPutRequestBody()
additionalData = [
'id' => 'SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7', 
'@odata.etag' => '1a371e53-f0a6-4327-a1ee-e3c56e4b38aa', 
'availability' => availability1 = ()
availability1Recurrence = Recurrence()
availability1RecurrencePattern = Pattern()
		availability1RecurrencePattern.setType('Weekly')

availability1RecurrencePattern.setDaysOfWeek(['Monday', 'Wednesday', 'Friday', ])

	availability1RecurrencePattern.setInterval(1)


availability1Recurrence.setPattern($availability1RecurrencePattern)
availability1RecurrenceRange = Range()
	availability1RecurrenceRange.setType('noEnd')


availability1Recurrence.setRange($availability1RecurrenceRange)

availability1.setRecurrence($availability1Recurrence)
	availability1.setTimeZone('Pacific Standard Time')

	availability1.setTimeSlots(null)


availabilityArray []= availability1;
request_body.setAvailability(availabilityArray)


];
request_body.setAdditionalData(additionalData)




await client.usersById('user-id').settings.shiftPreferences.put(request_body)


```