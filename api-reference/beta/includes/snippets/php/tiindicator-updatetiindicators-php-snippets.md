---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ValueRequestBody();


$valueArray = [];

$valuevalue1 = new TiIndicator();

$valuevalue1AdditionalData = [
	"id" => 'c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4',
	"additionalInformation" => 'mytest',
];
$valuevalue1->setAdditionalData($valuevalue1AdditionalData);

$valueArray []= $valuevalue1;

$valuevalue2 = new TiIndicator();

$valuevalue2AdditionalData = [
"id" => 'e58c072b-c9bb-a5c4-34ce-eb69af44fb1e',
"additionalInformation" => 'test again',
];
$valuevalue2->setAdditionalData($valuevalue2AdditionalData);

$valueArray []= $valuevalue2;
$requestRequestBody->setValue($valueArray);
$result =  $graphClient->security()->tiIndicators()->updateTiIndicators()->post($requestRequestBody);


```