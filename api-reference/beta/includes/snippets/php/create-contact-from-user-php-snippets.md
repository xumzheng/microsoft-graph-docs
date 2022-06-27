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

$emailAddressesemailAddresses1 = new TypedEmailAddress();

$emailAddressesemailAddresses1AdditionalData = [
	"address" => 'pavelb@contoso.onmicrosoft.com',
	"name" => 'Pavel Bansky',
	"type" => 'personal',
];
$emailAddressesemailAddresses1->setAdditionalData($emailAddressesemailAddresses1AdditionalData);

$emailAddressesArray []= $emailAddressesemailAddresses1;

$emailAddressesemailAddresses2 = new TypedEmailAddress();

$emailAddressesemailAddresses2AdditionalData = [
"address" => 'pavelb@fabrikam.onmicrosoft.com',
"name" => 'Pavel Bansky',
"type" => 'other',
"otherLabel" => 'Volunteer work',
];
$emailAddressesemailAddresses2->setAdditionalData($emailAddressesemailAddresses2AdditionalData);

$emailAddressesArray []= $emailAddressesemailAddresses2;
$requestRequestBody->setEmailAddresses($emailAddressesArray);
$phonesArray = [];

$phonesphones1 = new Phone();

$phonesphones1->setNumber('+1 732 555 0102');
$phonesphones1->setType(new PhoneType('business'));

$phonesArray []= $phonesphones1;
$requestRequestBody->setPhones($phonesArray);
$result =  $graphClient->me()->contacts()->post($requestRequestBody);


```