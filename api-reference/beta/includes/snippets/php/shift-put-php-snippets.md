---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Shift-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => 'SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8',
	"createdDateTime" => '2019-03-14T04:32:51.451Z',
	"lastModifiedDateTime" => '2019-03-14T05:32:51.451Z',
	"userId" => 'c5d0c76b-80c4-481c-be50-923cd8d680a1',
	"schedulingGroupId" => 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$requestConfiguration = new ShiftRequestBuilderPutRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->teamsById('team-id')->schedule()->shiftsById('shift-id')->put($requestRequestBody, $requestConfiguration);


```