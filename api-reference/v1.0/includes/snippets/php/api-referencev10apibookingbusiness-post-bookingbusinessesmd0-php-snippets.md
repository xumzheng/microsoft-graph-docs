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


$address->setStreet('4567 Main Street');
$address->setCity('Buffalo');
$address->setState('NY');
$address->setCountryOrRegion('USA');
$address->setPostalCode('98052');
$addressAdditionalData = [
	"postOfficeBox" => 'P.O. Box 123',
];
$address->setAdditionalData($addressAdditionalData);

$requestRequestBody->setPhone('206-555-0100');
$requestRequestBody->setEmail('manager@fourthcoffee.com');
$requestRequestBody->setWebSiteUrl('https://www.fourthcoffee.com');
$requestRequestBody->setDefaultCurrencyIso('USD');
$result =  $graphClient->solutions()->bookingBusinesses()->post($requestRequestBody);


```