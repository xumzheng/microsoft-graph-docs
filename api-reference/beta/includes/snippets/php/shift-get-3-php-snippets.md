---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ShiftPreferencesPutRequestBody();


$requestRequestBodyAdditionalData = [
	"id" => 'SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7',
	"@odata.etag" => '1a371e53-f0a6-4327-a1ee-e3c56e4b38aa',
	"availability" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->usersById('user-id')->settings()->shiftPreferences()->put($requestRequestBody);


```