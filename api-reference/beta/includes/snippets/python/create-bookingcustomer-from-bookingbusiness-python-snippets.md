---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomer()
request_body.setDisplayName('Joni Sherman')

request_body.setEmailAddress('jonis@relecloud.com')

addressesPhysicalAddress1 = PhysicalAddress()
addressesPhysicalAddress1.setPostOfficeBox('')

addressesPhysicalAddress1.setStreet('4567 Main Street')

addressesPhysicalAddress1.setCity('Buffalo')

addressesPhysicalAddress1.setState('NY')

addressesPhysicalAddress1.setCountryOrRegion('USA')

addressesPhysicalAddress1.setPostalCode('98052')

addressesPhysicalAddress1.setType(PhysicalAddressType('home'))


addressesArray []= addressesPhysicalAddress1;
addressesPhysicalAddress2 = PhysicalAddress()
addressesPhysicalAddress2.setPostOfficeBox('')

addressesPhysicalAddress2.setStreet('4570 Main Street')

addressesPhysicalAddress2.setCity('Buffalo')

addressesPhysicalAddress2.setState('NY')

addressesPhysicalAddress2.setCountryOrRegion('USA')

addressesPhysicalAddress2.setPostalCode('98054')

addressesPhysicalAddress2.setType(PhysicalAddressType('business'))


addressesArray []= addressesPhysicalAddress2;
request_body.setAddresses(addressesArray)


phonesPhone1 = Phone()
phonesPhone1.setNumber('206-555-0100')

phonesPhone1.setType(PhoneType('home'))


phonesArray []= phonesPhone1;
phonesPhone2 = Phone()
phonesPhone2.setNumber('206-555-0200')

phonesPhone2.setType(PhoneType('business'))


phonesArray []= phonesPhone2;
request_body.setPhones(phonesArray)



request_config = CustomersRequestBuilderPostRequestConfiguration(
request_config = CustomersRequestBuilderPostRequestConfiguration(query_params=)


result = await client.bookingBusinesses_by_id('bookingBusiness-id').customers.post(request_body, headers=)


```