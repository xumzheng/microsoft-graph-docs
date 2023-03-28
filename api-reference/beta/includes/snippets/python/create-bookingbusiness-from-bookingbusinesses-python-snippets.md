---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new BookingBusiness();
$requestBody->setDisplayName('Fourth Coffee');

$address = new PhysicalAddress();
$address->setPostOfficeBox('P.O. Box 123');

$address->setStreet('4567 Main Street');

$address->setCity('Buffalo');

$address->setState('NY');

$address->setCountryOrRegion('USA');

$address->setPostalCode('98052');


$requestBody->setAddress($address);
$requestBody->setPhone('206-555-0100');

$requestBody->setEmail('manager@fourthcoffee.com');

$requestBody->setWebSiteUrl('https://www.fourthcoffee.com');

$requestBody->setDefaultCurrencyIso('USD');



$requestResult = $graphServiceClient->bookingBusinesses()->post($requestBody);


```