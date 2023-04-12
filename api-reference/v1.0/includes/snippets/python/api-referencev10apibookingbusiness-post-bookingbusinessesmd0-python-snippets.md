---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingBusiness()
request_body.displayName = 'Fourth Coffee'

address = PhysicalAddress()
address.street = '4567 Main Street'

address.city = 'Buffalo'

address.state = 'NY'

address.countryOrRegion = 'USA'

address.postalCode = '98052'

additionalData = [
'postOfficeBox' => 'P.O. Box 123', 
];
address.additionaldata(additionalData)



request_body.address = address
request_body.phone = '206-555-0100'

request_body.email = 'manager@fourthcoffee.com'

request_body.webSiteUrl = 'https://www.fourthcoffee.com'

request_body.defaultCurrencyIso = 'USD'




result = await client.solutions.bookingBusinesses.post(request_body = request_body)


```