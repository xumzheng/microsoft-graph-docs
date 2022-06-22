---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OfferShiftRequest();


$requestRequestBody->setSenderShiftId('SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29');
$requestRequestBody->setSenderMessage('Having a family emergency, could you take this shift for me?');
$requestRequestBody->setRecipientUserId('fe278b61-21ac-4872-8b41-1962bbb98e3c');
$requestConfiguration = new OfferShiftRequestsRequestBuilderPostRequestConfiguration();

$headers = [
"Authorization" => "Bearer {token}",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->teamsById('team-id')->schedule()->offerShiftRequests()->post($requestRequestBody, $requestConfiguration);


```