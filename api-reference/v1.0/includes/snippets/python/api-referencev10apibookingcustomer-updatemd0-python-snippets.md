---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = BookingCustomerBase();
requestBody.set@odatatype('#microsoft.graph.bookingCustomer');

additionalData = [
'displayName' => 'Adele', 
'emailAddress' => 'adele@relecloud.com', 
];
requestBody.setAdditionalData(additionalData);




result = await client.solutions().bookingBusinessesById('bookingBusiness-id').customersById('bookingCustomerBase-id').patch(requestBody);


```