---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ItemAddress();
request_body.setDisplayName('Home');

detail = PhysicalAddress();
detail.setType(PhysicalAddressType('home'));

Detail.setPostOfficeBox(null);

detail.setStreet('221B Baker Street');

detail.setCity('London');

Detail.setState(null);

detail.setCountryOrRegion('United Kingdom');

detail.setPostalCode('E14 3TD');


request_body.setDetail($detail);


result = await client.me.profile.addresses.post(request_body);


```