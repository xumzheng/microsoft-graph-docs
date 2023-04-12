---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CancelPostRequestBody()
request_body.cancellationMessage = 'Your appointment has been successfully cancelled. Please call us again.'




await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').appointments_by_id('bookingAppointment-id').cancel.post(request_body = request_body)


```