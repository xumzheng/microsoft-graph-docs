---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingCustomer();


$requestRequestBody->setDisplayName('Joni Sherman');
$requestRequestBody->setEmailAddress('jonis@relecloud.com');
$addressesArray = [];

$addressesaddresses1 = new PhysicalAddress();

$addressesaddresses1->setPostOfficeBox('');
$addressesaddresses1->setStreet('4567 Main Street');
$addressesaddresses1->setCity('Buffalo');
$addressesaddresses1->setState('NY');
$addressesaddresses1->setCountryOrRegion('USA');
$addressesaddresses1->setPostalCode('98052');
$addressesaddresses1->setType(new PhysicalAddressType('home'));

$addressesArray []= $addressesaddresses1;

$addressesaddresses2 = new PhysicalAddress();

$addressesaddresses2->setPostOfficeBox('');
$addressesaddresses2->setStreet('4570 Main Street');
$addressesaddresses2->setCity('Buffalo');
$addressesaddresses2->setState('NY');
$addressesaddresses2->setCountryOrRegion('USA');
$addressesaddresses2->setPostalCode('98054');
$addressesaddresses2->setType(new PhysicalAddressType('business'));

$addressesArray []= $addressesaddresses2;
$requestRequestBody->setAddresses($addressesArray);
$phonesArray = [];

$phonesphones1 = new Phone();

$phonesphones1->setNumber('206-555-0100');
$phonesphones1->setType(new PhoneType('home'));

$phonesArray []= $phonesphones1;

$phonesphones2 = new Phone();

$phonesphones2->setNumber('206-555-0200');
$phonesphones2->setType(new PhoneType('business'));

$phonesArray []= $phonesphones2;
$requestRequestBody->setPhones($phonesArray);
$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->customers()->post($requestRequestBody);


```