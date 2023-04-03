---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = BookingCustomer();
requestBody.setDisplayName('Adele');

requestBody.setEmailAddress('adele@relecloud.com');



requestResult = graphServiceClient.bookingBusinessesById('bookingBusiness-id').customersById('bookingCustomer-id').patch(requestBody);


```