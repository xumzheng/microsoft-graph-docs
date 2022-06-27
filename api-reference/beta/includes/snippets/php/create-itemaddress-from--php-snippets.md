---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ItemAddress();


$requestRequestBody->setDisplayName('Home');

$detail = new PhysicalAddress();
$requestRequestBody->setDetail($detail);


$detail->setType(new PhysicalAddressType('home'));
$detail->setPostOfficeBox(null);
$detail->setStreet('221B Baker Street');
$detail->setCity('London');
$detail->setState(null);
$detail->setCountryOrRegion('United Kingdom');
$detail->setPostalCode('E14 3TD');

$result =  $graphClient->me()->profile()->addresses()->post($requestRequestBody);


```