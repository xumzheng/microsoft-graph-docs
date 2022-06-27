---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TimeOff-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"userId" => 'c5d0c76b-80c4-481c-be50-923cd8d680a1',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$requestConfiguration = new TimeOffRequestBuilderPutRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->teamsById('team-id')->schedule()->timesOffById('timeOff-id')->put($requestRequestBody, $requestConfiguration);


```