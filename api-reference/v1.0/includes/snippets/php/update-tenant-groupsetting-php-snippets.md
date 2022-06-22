---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GroupSetting();


$valuesArray = [];

$values1 = new SettingValue();

$values1AdditionalData = [
		"name" => 'AllowToAddGuests',
		"value" => 'false',
	];
$values1->setAdditionalData($values1AdditionalData);

$valuesArray []= $values1;
$requestRequestBody->setValues($valuesArray);
$result =  $graphClient->groupSettingsById('groupSetting-id')->patch($requestRequestBody);


```