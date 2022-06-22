---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DirectorySetting();


$requestRequestBody->setTemplateId('62375ab9-6b52-47ed-826b-58e47e0e304b');
$valuesArray = [];

$values1 = new SettingValue();

$values1AdditionalData = [
		"name" => 'GuestUsageGuidelinesUrl',
		"value" => 'https://privacy.contoso.com/privacystatement',
	];
$values1->setAdditionalData($values1AdditionalData);

$valuesArray []= $values1;

$values2 = new SettingValue();

$values2AdditionalData = [
	"name" => 'EnableMSStandardBlockedWords',
	"value" => 'true',
];
$values2->setAdditionalData($values2AdditionalData);

$valuesArray []= $values2;

$values3 = new SettingValue();

$values3AdditionalData = [
"name" => 'EnableMIPLabels',
"value" => 'true',
];
$values3->setAdditionalData($values3AdditionalData);

$valuesArray []= $values3;

$values4 = new SettingValue();

$values4AdditionalData = [
"name" => 'PrefixSuffixNamingRequirement',
"value" => '[Contoso-][GroupName]',
];
$values4->setAdditionalData($values4AdditionalData);

$valuesArray []= $values4;
$requestRequestBody->setValues($valuesArray);
$result =  $graphClient->settings()->post($requestRequestBody);


```