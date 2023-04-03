---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = BookingCustomer();
requestBody.setDisplayName('Adele');

requestBody.setEmailAddress('adele@relecloud.com');



result = await client.bookingBusinessesById('bookingBusiness-id').customersById('bookingCustomer-id').patch(requestBody);


```