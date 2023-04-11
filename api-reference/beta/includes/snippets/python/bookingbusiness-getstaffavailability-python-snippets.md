---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetStaffAvailabilityPostRequestBody()
request_body.StaffIds(['311a5454-08b2-4560-ba1c-f715e938cb79', ])

startDateTime = DateTimeTimeZone()
startDateTime.dateTime = '2022-01-25T00:00:00'

startDateTime.timeZone = 'India Standard Time'


request_body.startDateTime = startDateTime
endDateTime = DateTimeTimeZone()
endDateTime.dateTime = '2022-01-26T17:00:00'

endDateTime.timeZone = 'Pacific Standard Time'


request_body.endDateTime = endDateTime



result = await client.bookingBusinesses_by_id('bookingBusiness-id').getStaffAvailability.post(request_body = request_body)


```