---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingCustomer();


$requestRequestBody->setDisplayName('Adele');
$requestRequestBody->setEmailAddress('adele@relecloud.com');
$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->customersById('bookingCustomer-id')->patch($requestRequestBody);


```