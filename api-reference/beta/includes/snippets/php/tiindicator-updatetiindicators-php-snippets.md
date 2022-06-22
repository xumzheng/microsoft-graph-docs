---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ValueRequestBody();


$valueArray = [];

$value1 = new TiIndicator();

$value1AdditionalData = [
		"id" => 'c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4',
		"additionalInformation" => 'mytest',
	];
$value1->setAdditionalData($value1AdditionalData);

$valueArray []= $value1;

$value2 = new TiIndicator();

$value2AdditionalData = [
	"id" => 'e58c072b-c9bb-a5c4-34ce-eb69af44fb1e',
	"additionalInformation" => 'test again',
];
$value2->setAdditionalData($value2AdditionalData);

$valueArray []= $value2;
$requestRequestBody->setValue($valueArray);
$result =  $graphClient->security()->tiIndicators()->updateTiIndicators()->post($requestRequestBody);


```