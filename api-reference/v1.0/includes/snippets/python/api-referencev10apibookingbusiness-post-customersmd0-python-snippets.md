---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomerBase()
request_body.@odatatype = '#microsoft.graph.bookingCustomer'

additionalData = [
'displayName' => 'Joni Sherman', 
'emailAddress' => 'jonis@relecloud.com', 
'addresses' => addresses1 = ()
		addresses1.postOfficeBox = ''

		addresses1.street = '4567 Main Street'

		addresses1.city = 'Buffalo'

		addresses1.state = 'NY'

		addresses1.countryOrRegion = 'USA'

		addresses1.postalCode = '98052'

		addresses1.type = 'home'


addressesArray []= addresses1;
addresses2 = ()
		addresses2.postOfficeBox = ''

		addresses2.street = '4570 Main Street'

		addresses2.city = 'Buffalo'

		addresses2.state = 'NY'

		addresses2.countryOrRegion = 'USA'

		addresses2.postalCode = '98054'

		addresses2.type = 'business'


addressesArray []= addresses2;
request_body.addresses(addressesArray)


'phones' => phones1 = ()
	phones1.number = '206-555-0100'

	phones1.type = 'home'


phonesArray []= phones1;
phones2 = ()
	phones2.number = '206-555-0200'

	phones2.type = 'business'


phonesArray []= phones2;
request_body.phones(phonesArray)


];
request_body.additionaldata(additionalData)





result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').customers.post(request_body = request_body)


```