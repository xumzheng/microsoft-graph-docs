---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DirectorySetting();


$valuesArray = [];

$valuesvalues1 = new SettingValue();

$valuesvalues1AdditionalData = [
	"name" => 'CustomBlockedWordsList',
	"value" => 'Contoso',
];
$valuesvalues1->setAdditionalData($valuesvalues1AdditionalData);

$valuesArray []= $valuesvalues1;
$requestRequestBody->setValues($valuesArray);
$result =  $graphClient->settingsById('directorySetting-id')->patch($requestRequestBody);


```