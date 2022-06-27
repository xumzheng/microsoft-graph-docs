---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Contact();



$homeAddress = new PhysicalAddress();
$requestRequestBody->setHomeAddress($homeAddress);


$homeAddress->setStreet('123 Some street');
$homeAddress->setCity('Seattle');
$homeAddress->setState('WA');
$homeAddress->setPostalCode('98121');

$requestRequestBody->setBirthday(new DateTime("1974-07-22"));
$result =  $graphClient->me()->contactsById('contact-id')->patch($requestRequestBody);


```