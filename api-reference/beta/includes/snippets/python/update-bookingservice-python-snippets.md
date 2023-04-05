---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingService()
request_body.set@odatatype('#microsoft.graph.bookingService')

$request_body.setDefaultDuration( \DateInterval('PT30M'))



result = await client.bookingBusinesses._by_id('bookingBusiness-id').services._by_id('bookingService-id').patch(request_body)


```