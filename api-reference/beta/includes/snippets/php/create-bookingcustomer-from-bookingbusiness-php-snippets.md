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

$addresses1 = new PhysicalAddress();

$addresses1->setPostOfficeBox('');
$addresses1->setStreet('4567 Main Street');
$addresses1->setCity('Buffalo');
$addresses1->setState('NY');
$addresses1->setCountryOrRegion('USA');
$addresses1->setPostalCode('98052');
$addresses1->setType(new PhysicalAddressType('home'));

$addressesArray []= $addresses1;

$addresses2 = new PhysicalAddress();

$addresses2->setPostOfficeBox('');
$addresses2->setStreet('4570 Main Street');
$addresses2->setCity('Buffalo');
$addresses2->setState('NY');
$addresses2->setCountryOrRegion('USA');
$addresses2->setPostalCode('98054');
$addresses2->setType(new PhysicalAddressType('business'));

$addressesArray []= $addresses2;
$requestRequestBody->setAddresses($addressesArray);
$phonesArray = [];

$phones1 = new Phone();

$phones1->setNumber('206-555-0100');
$phones1->setType(new PhoneType('home'));

$phonesArray []= $phones1;

$phones2 = new Phone();

$phones2->setNumber('206-555-0200');
$phones2->setType(new PhoneType('business'));

$phonesArray []= $phones2;
$requestRequestBody->setPhones($phonesArray);
$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->customers()->post($requestRequestBody);


```