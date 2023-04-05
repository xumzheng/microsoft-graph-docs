---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingService()
request_body.set@odatatype('#microsoft.graph.bookingService')

$request_body.setDefaultDuration( \DateInterval('PT30M'))



result = await client.solutions_bookingBusinessesby_id('bookingBusiness-id')_servicesby_id('bookingService-id').patch(request_body)


```