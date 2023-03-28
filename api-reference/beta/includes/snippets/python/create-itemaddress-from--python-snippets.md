---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ItemAddress();
$requestBody->setDisplayName('Home');

$detail = new PhysicalAddress();
$detail->setType(new PhysicalAddressType('home'));

$Detail->setPostOfficeBox(null);

$detail->setStreet('221B Baker Street');

$detail->setCity('London');

$Detail->setState(null);

$detail->setCountryOrRegion('United Kingdom');

$detail->setPostalCode('E14 3TD');


$requestBody->setDetail($detail);


$requestResult = $graphServiceClient->me()->profile()->addresses()->post($requestBody);


```