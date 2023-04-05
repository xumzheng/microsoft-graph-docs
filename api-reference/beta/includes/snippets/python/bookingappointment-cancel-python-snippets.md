---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CancelPostRequestBody()
request_body.setCancellationMessage('Your appointment has been successfully cancelled. Please call us again.')



await client.bookingBusinessesby_id('bookingBusiness-id').appointmentsby_id('bookingAppointment-id').cancel.post(request_body)


```