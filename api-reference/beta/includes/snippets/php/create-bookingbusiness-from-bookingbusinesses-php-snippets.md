---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingBusiness();


$requestRequestBody->setDisplayName('Fourth Coffee');

$address = new PhysicalAddress();
$requestRequestBody->setAddress($address);


$address->setPostOfficeBox('P.O. Box 123');
$address->setStreet('4567 Main Street');
$address->setCity('Buffalo');
$address->setState('NY');
$address->setCountryOrRegion('USA');
$address->setPostalCode('98052');

$requestRequestBody->setPhone('206-555-0100');
$requestRequestBody->setEmail('manager@fourthcoffee.com');
$requestRequestBody->setWebSiteUrl('https://www.fourthcoffee.com');
$requestRequestBody->setDefaultCurrencyIso('USD');
$result =  $graphClient->bookingBusinesses()->post($requestRequestBody);


```