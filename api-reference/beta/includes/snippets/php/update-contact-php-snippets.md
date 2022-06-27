---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Contact();


$emailAddressesArray = [];

$emailAddressesemailAddresses1 = new TypedEmailAddress();

$emailAddressesemailAddresses1AdditionalData = [
	"type" => 'personal',
	"name" => 'Pavel Bansky',
	"address" => 'pavelb@adatum.onmicrosoft.com',
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
$result =  $graphClient->me()->contactsById('contact-id')->patch($requestRequestBody);


```