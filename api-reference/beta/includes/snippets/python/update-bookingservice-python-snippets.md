---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new BookingService();
$requestBody.set@odatatype('#microsoft.graph.bookingService');

$requestBody.setDefaultDuration(new \DateInterval('PT30M'));



$requestResult = $graphServiceClient.bookingBusinessesById('bookingBusiness-id').servicesById('bookingService-id').patch($requestBody);


```