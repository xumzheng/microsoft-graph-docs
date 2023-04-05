---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetStaffAvailabilityPostRequestBody()
request_body.setStaffIds(['311a5454-08b2-4560-ba1c-f715e938cb79', ])

startDateTime = DateTimeTimeZone()
startDateTime.setDateTime('2022-01-25T00:00:00')

startDateTime.setTimeZone('India Standard Time')


request_body.setStartDateTime($startDateTime)
endDateTime = DateTimeTimeZone()
endDateTime.setDateTime('2022-01-26T17:00:00')

endDateTime.setTimeZone('Pacific Standard Time')


request_body.setEndDateTime($endDateTime)


result = await client.solutions.bookingBusinessesById('bookingBusiness-id').getStaffAvailability.post(request_body)


```