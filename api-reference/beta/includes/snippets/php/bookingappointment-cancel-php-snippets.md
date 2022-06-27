---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CancellationMessageRequestBody();


$requestRequestBody->setCancellationMessage('Your appointment has been successfully cancelled. Please call us again.');
$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->appointmentsById('bookingAppointment-id')->cancel()->post($requestRequestBody);


```