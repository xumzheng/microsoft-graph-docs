---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TimeOffReason-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"displayName" => 'Vacation',
	"iconType" => 'plane',
	"isActive" => True,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$requestConfiguration = new TimeOffReasonRequestBuilderPutRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->teamsById('team-id')->schedule()->timeOffReasonsById('timeOffReason-id')->put($requestRequestBody, $requestConfiguration);


```