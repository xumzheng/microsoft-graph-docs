---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = BookingBusiness();
request_body.setDisplayName('Fourth Coffee');

address = PhysicalAddress();
address.setStreet('4567 Main Street');

address.setCity('Buffalo');

address.setState('NY');

address.setCountryOrRegion('USA');

address.setPostalCode('98052');

additionalData = [
'postOfficeBox' => 'P.O. Box 123', 
];
address.setAdditionalData(additionalData);



request_body.setAddress($address);
request_body.setPhone('206-555-0100');

request_body.setEmail('manager@fourthcoffee.com');

request_body.setWebSiteUrl('https://www.fourthcoffee.com');

request_body.setDefaultCurrencyIso('USD');



result = await client.solutions().bookingBusinesses().post(request_body);


```