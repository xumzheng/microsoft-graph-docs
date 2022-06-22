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

$emailAddresses1 = new EmailAddress();

$emailAddresses1->setAddress('pavelb@fabrikam.onmicrosoft.com');
$emailAddresses1->setName('Pavel Bansky');

$emailAddressesArray []= $emailAddresses1;
$requestRequestBody->setEmailAddresses($emailAddressesArray);
$requestRequestBody->setBusinessPhones( [
'+1 732 555 0102',],
$result =  $graphClient->me()->contacts()->post($requestRequestBody);


```