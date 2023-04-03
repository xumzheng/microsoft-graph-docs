---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ItemAddress();
requestBody.setDisplayName('Home');

detail = PhysicalAddress();
detail.setType(PhysicalAddressType('home'));

Detail.setPostOfficeBox(null);

detail.setStreet('221B Baker Street');

detail.setCity('London');

Detail.setState(null);

detail.setCountryOrRegion('United Kingdom');

detail.setPostalCode('E14 3TD');


requestBody.setDetail($detail);


requestResult = graphServiceClient.me().profile().addresses().post(requestBody);


```