---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GroupSetting();


$requestRequestBody->setTemplateId('62375ab9-6b52-47ed-826b-58e47e0e304b');
$valuesArray = [];

$valuesvalues1 = new SettingValue();

$valuesvalues1AdditionalData = [
	"name" => 'GuestUsageGuidelinesUrl',
	"value" => 'https://privacy.contoso.com/privacystatement',
];
$valuesvalues1->setAdditionalData($valuesvalues1AdditionalData);

$valuesArray []= $valuesvalues1;

$valuesvalues2 = new SettingValue();

$valuesvalues2AdditionalData = [
"name" => 'EnableMSStandardBlockedWords',
"value" => 'true',
];
$valuesvalues2->setAdditionalData($valuesvalues2AdditionalData);

$valuesArray []= $valuesvalues2;

$valuesvalues3 = new SettingValue();

$valuesvalues3AdditionalData = [
"name" => 'EnableMIPLabels',
"value" => 'true',
];
$valuesvalues3->setAdditionalData($valuesvalues3AdditionalData);

$valuesArray []= $valuesvalues3;

$valuesvalues4 = new SettingValue();

$valuesvalues4AdditionalData = [
"name" => 'PrefixSuffixNamingRequirement',
"value" => '[Contoso-][GroupName]',
];
$valuesvalues4->setAdditionalData($valuesvalues4AdditionalData);

$valuesArray []= $valuesvalues4;
$requestRequestBody->setValues($valuesArray);
$result =  $graphClient->groupSettings()->post($requestRequestBody);


```