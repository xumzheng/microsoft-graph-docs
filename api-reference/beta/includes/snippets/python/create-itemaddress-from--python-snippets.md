---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ItemAddress()
request_body.displayName = 'Home'

detail = PhysicalAddress()
detail.Type(PhysicalAddressType('home'))

Detail.postOfficeBox=null

detail.street = '221B Baker Street'

detail.city = 'London'

Detail.state=null

detail.countryOrRegion = 'United Kingdom'

detail.postalCode = 'E14 3TD'


request_body.detail = detail


request_configuration = AddressesRequestBuilderPostRequestConfiguration(
)


result = await client.me.profile.addresses.post(request_body = request_body)


```