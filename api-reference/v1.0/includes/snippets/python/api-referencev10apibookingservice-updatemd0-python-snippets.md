---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingService()
request_body.set@odatatype('#microsoft.graph.bookingService')

$request_body.setDefaultDuration( \DateInterval('PT30M'))


request_config = BookingServiceRequestBuilderPatchRequestConfiguration(
request_config = BookingServiceRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').services_by_id('bookingService-id').patch(request_body, headers=)


```