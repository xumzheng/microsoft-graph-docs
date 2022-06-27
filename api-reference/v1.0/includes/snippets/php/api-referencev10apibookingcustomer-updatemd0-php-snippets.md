---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingCustomerBase();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingCustomer',
	"displayName" => 'Adele',
	"emailAddress" => 'adele@relecloud.com',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->solutions()->bookingBusinessesById('bookingBusiness-id')->customersById('bookingCustomerBase-id')->patch($requestRequestBody);


```