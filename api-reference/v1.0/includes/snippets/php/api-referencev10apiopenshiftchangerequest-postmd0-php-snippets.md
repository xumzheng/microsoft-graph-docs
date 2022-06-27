---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OpenShiftChangeRequest();


$requestRequestBody->setSenderMessage('Can I take this shift?');
$requestRequestBody->setOpenShiftId('577b75d2-a927-48c0-a5d1-dc984894e7b8');
$requestConfiguration = new OpenShiftChangeRequestsRequestBuilderPostRequestConfiguration();

$headers = [
"Authorization" => "Bearer {token}",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->teamsById('team-id')->schedule()->openShiftChangeRequests()->post($requestRequestBody, $requestConfiguration);


```