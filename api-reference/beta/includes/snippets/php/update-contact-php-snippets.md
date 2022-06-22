---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Contact();


$emailAddressesArray = [];

$emailAddresses1 = new TypedEmailAddress();

$emailAddresses1AdditionalData = [
		"type" => 'personal',
		"name" => 'Pavel Bansky',
		"address" => 'pavelb@adatum.onmicrosoft.com',
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
$result =  $graphClient->me()->contactsById('contact-id')->patch($requestRequestBody);


```