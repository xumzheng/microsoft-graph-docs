---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SwapShiftsChangeRequest();


$requestRequestBody->setSenderShiftId('5ad10161-6524-4c7c-9beb-4e8677ba2f6d');
$requestRequestBody->setSenderMessage('I can\'t make my shift, any chance we can swap?');
$requestRequestBody->setRecipientUserId('567c8ea5-9e32-422a-a663-8270201699cd');
$requestRequestBody->setRecipientShiftId('e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c');
$requestConfiguration = new SwapShiftsChangeRequestsRequestBuilderPostRequestConfiguration();

$headers = [
"Authorization" => "Bearer {token}",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->teamsById('team-id')->schedule()->swapShiftsChangeRequests()->post($requestRequestBody, $requestConfiguration);


```