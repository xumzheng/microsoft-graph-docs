---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomerBase()
request_body.@odatatype = '#microsoft.graph.bookingCustomer'

additionalData = [
'displayName' => 'Adele', 
'emailAddress' => 'adele@relecloud.com', 
];
request_body.additionaldata(additionalData)





result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').customers_by_id('bookingCustomerBase-id').patch(request_body = request_body)


```