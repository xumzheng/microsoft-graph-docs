---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomer()
request_body.setDisplayName('Adele')

request_body.setEmailAddress('adele@relecloud.com')



result = await client.bookingBusinessesById('bookingBusiness-id').customersById('bookingCustomer-id').patch(request_body)


```