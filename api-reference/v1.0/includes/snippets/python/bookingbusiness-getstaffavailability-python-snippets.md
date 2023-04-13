---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetStaffAvailabilityPostRequestBody()
request_body.StaffIds(['311a5454-08b2-4560-ba1c-f715e938cb79', ])

start_date_time = DateTimeTimeZone()
startDateTime.dateTime = '2022-01-25T00:00:00'

startDateTime.timeZone = 'India Standard Time'


request_body.start_date_time = startDateTime
end_date_time = DateTimeTimeZone()
endDateTime.dateTime = '2022-01-26T17:00:00'

endDateTime.timeZone = 'Pacific Standard Time'


request_body.end_date_time = endDateTime



result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').getStaffAvailability.post(request_body = request_body)


```