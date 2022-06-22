---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Contact();


$requestRequestBody->setGivenName('Pavel');
$requestRequestBody->setSurname('Bansky');
$emailAddressesArray = [];

$emailAddresses1 = new TypedEmailAddress();

$emailAddresses1AdditionalData = [
		"address" => 'pavelb@contoso.onmicrosoft.com',
		"name" => 'Pavel Bansky',
		"type" => 'personal',
	];
$emailAddresses1->setAdditionalData($emailAddresses1AdditionalData);

$emailAddressesArray []= $emailAddresses1;

$emailAddresses2 = new TypedEmailAddress();

$emailAddresses2AdditionalData = [
	"address" => 'pavelb@fabrikam.onmicrosoft.com',
	"name" => 'Pavel Bansky',
	"type" => 'other',
	"otherLabel" => 'Volunteer work',
];
$emailAddresses2->setAdditionalData($emailAddresses2AdditionalData);

$emailAddressesArray []= $emailAddresses2;
$requestRequestBody->setEmailAddresses($emailAddressesArray);
$phonesArray = [];

$phones1 = new Phone();

$phones1->setNumber('+1 732 555 0102');
$phones1->setType(new PhoneType('business'));

$phonesArray []= $phones1;
$requestRequestBody->setPhones($phonesArray);
$result =  $graphClient->me()->contacts()->post($requestRequestBody);


```