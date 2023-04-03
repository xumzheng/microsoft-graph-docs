---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CancelPostRequestBody();
requestBody.setCancellationMessage('Your appointment has been successfully cancelled. Please call us again.');



awaitclient.bookingBusinessesById('bookingBusiness-id').appointmentsById('bookingAppointment-id').cancel().post(requestBody);


```