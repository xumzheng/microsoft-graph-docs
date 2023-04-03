---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BookingService();
requestBody.set@odatatype('#microsoft.graph.bookingService');

$requestBody.setDefaultDuration( \DateInterval('PT30M'));



result = awaitclient.bookingBusinessesById('bookingBusiness-id').servicesById('bookingService-id').patch(requestBody);


```