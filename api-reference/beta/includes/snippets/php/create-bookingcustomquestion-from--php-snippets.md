---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingCustomQuestion-idPostRequestBody();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingCustomQuestion',
	"displayName" => 'What is your age?',
	"answerInputType" => 'text',
	"answerOptions" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->customQuestionsById('bookingCustomQuestion-id')->post($requestRequestBody);


```