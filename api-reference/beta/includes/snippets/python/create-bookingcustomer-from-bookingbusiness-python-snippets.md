---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingCustomer()
request_body.displayName = 'Joni Sherman'

request_body.emailAddress = 'jonis@relecloud.com'

addressesPhysicalAddress1 = PhysicalAddress()
addressesPhysicalAddress1.postOfficeBox = ''

addressesPhysicalAddress1.street = '4567 Main Street'

addressesPhysicalAddress1.city = 'Buffalo'

addressesPhysicalAddress1.state = 'NY'

addressesPhysicalAddress1.countryOrRegion = 'USA'

addressesPhysicalAddress1.postalCode = '98052'

addressesPhysicalAddress1.Type(PhysicalAddressType('home'))


addressesArray []= addressesPhysicalAddress1;
addressesPhysicalAddress2 = PhysicalAddress()
addressesPhysicalAddress2.postOfficeBox = ''

addressesPhysicalAddress2.street = '4570 Main Street'

addressesPhysicalAddress2.city = 'Buffalo'

addressesPhysicalAddress2.state = 'NY'

addressesPhysicalAddress2.countryOrRegion = 'USA'

addressesPhysicalAddress2.postalCode = '98054'

addressesPhysicalAddress2.Type(PhysicalAddressType('business'))


addressesArray []= addressesPhysicalAddress2;
request_body.addresses(addressesArray)


phonesPhone1 = Phone()
phonesPhone1.number = '206-555-0100'

phonesPhone1.Type(PhoneType('home'))


phonesArray []= phonesPhone1;
phonesPhone2 = Phone()
phonesPhone2.number = '206-555-0200'

phonesPhone2.Type(PhoneType('business'))


phonesArray []= phonesPhone2;
request_body.phones(phonesArray)




request_configuration = CustomersRequestBuilderPostRequestConfiguration(
)


result = await client.bookingBusinesses_by_id('bookingBusiness-id').customers.post(request_body = request_body)


```