---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomerBase()
request_body.set@odatatype('#microsoft.graph.bookingCustomer')

additionalData = [
'displayName' => 'Joni Sherman', 
'emailAddress' => 'jonis@relecloud.com', 
'addresses' => addresses1 = ()
		addresses1.setPostOfficeBox('')

		addresses1.setStreet('4567 Main Street')

		addresses1.setCity('Buffalo')

		addresses1.setState('NY')

		addresses1.setCountryOrRegion('USA')

		addresses1.setPostalCode('98052')

		addresses1.setType('home')


addressesArray []= addresses1;
addresses2 = ()
		addresses2.setPostOfficeBox('')

		addresses2.setStreet('4570 Main Street')

		addresses2.setCity('Buffalo')

		addresses2.setState('NY')

		addresses2.setCountryOrRegion('USA')

		addresses2.setPostalCode('98054')

		addresses2.setType('business')


addressesArray []= addresses2;
request_body.setAddresses(addressesArray)


'phones' => phones1 = ()
	phones1.setNumber('206-555-0100')

	phones1.setType('home')


phonesArray []= phones1;
phones2 = ()
	phones2.setNumber('206-555-0200')

	phones2.setType('business')


phonesArray []= phones2;
request_body.setPhones(phonesArray)


];
request_body.setAdditionalData(additionalData)



request_config = CustomersRequestBuilderPostRequestConfiguration(
request_config = CustomersRequestBuilderPostRequestConfiguration(query_params=)


result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').customers.post(request_body, headers=)


```