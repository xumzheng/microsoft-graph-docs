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
		availability1RecurrencePattern.type = 'Weekly'

availability1RecurrencePattern.DaysOfWeek(['Monday', 'Wednesday', 'Friday', ])

	availability1RecurrencePattern.interval = 1


availability1Recurrence.pattern = availability1RecurrencePattern
availability1RecurrenceRange = Range()
	availability1RecurrenceRange.type = 'noEnd'


availability1Recurrence.range = availability1RecurrenceRange

availability1.recurrence = availability1Recurrence
	availability1.timeZone = 'Pacific Standard Time'

	availability1.timeSlots=null


availabilityArray []= availability1;
request_body.availability(availabilityArray)


];
request_body.additionaldata(additionalData)




request_configuration = ShiftPreferencesRequestBuilderPutRequestConfiguration(
)


await client.users_by_id('user-id').settings.shiftPreferences.put(request_body = request_body)


```