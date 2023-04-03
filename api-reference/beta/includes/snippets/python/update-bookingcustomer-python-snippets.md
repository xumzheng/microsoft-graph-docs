---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BookingCustomer();
requestBody.setDisplayName('Adele');

requestBody.setEmailAddress('adele@relecloud.com');



result = awaitclient.bookingBusinessesById('bookingBusiness-id').customersById('bookingCustomer-id').patch(requestBody);


```