---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingService();


$requestRequestBody->setDefaultDuration('PT30M');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingService',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->solutions()->bookingBusinessesById('bookingBusiness-id')->servicesById('bookingService-id')->patch($requestRequestBody);


```