---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingCustomerBase();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingCustomer',
	"displayName" => 'Joni Sherman',
	"emailAddress" => 'jonis@relecloud.com',
	"addresses" => [],
"phones" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->solutions()->bookingBusinessesById('bookingBusiness-id')->customers()->post($requestRequestBody);


```