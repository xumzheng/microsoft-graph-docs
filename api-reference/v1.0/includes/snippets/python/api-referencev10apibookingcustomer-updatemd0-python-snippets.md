---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomerBase()
request_body.set@odatatype('#microsoft.graph.bookingCustomer')

additionalData = [
'displayName' => 'Adele', 
'emailAddress' => 'adele@relecloud.com', 
];
request_body.setAdditionalData(additionalData)




result = await client.solutions.bookingBusinesses._by_id('bookingBusiness-id').customers._by_id('bookingCustomerBase-id').patch(request_body)


```