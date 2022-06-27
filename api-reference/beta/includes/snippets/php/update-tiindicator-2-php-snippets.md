---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TiIndicator();


$requestRequestBody->setAdditionalInformation('additionalInformation-after-update');
$requestRequestBody->setConfidence(42);
$requestRequestBody->setDescription('description-after-update');
$requestConfiguration = new TiIndicatorRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->security()->tiIndicatorsById('tiIndicator-id')->patch($requestRequestBody, $requestConfiguration);


```