---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GroupSetting();


$valuesArray = [];

$valuesvalues1 = new SettingValue();

$valuesvalues1AdditionalData = [
	"name" => 'AllowToAddGuests',
	"value" => 'true',
];
$valuesvalues1->setAdditionalData($valuesvalues1AdditionalData);

$valuesArray []= $valuesvalues1;
$requestRequestBody->setValues($valuesArray);
$result =  $graphClient->groupsById('group-id')->settingsById('groupSetting-id')->patch($requestRequestBody);


```