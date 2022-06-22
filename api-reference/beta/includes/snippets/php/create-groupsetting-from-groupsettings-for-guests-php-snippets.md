---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DirectorySetting();


$requestRequestBody->setTemplateId('08d542b9-071f-4e16-94b0-74abb372e3d9');
$valuesArray = [];

$values1 = new SettingValue();

$values1AdditionalData = [
		"name" => 'AllowToAddGuests',
		"value" => 'false',
	];
$values1->setAdditionalData($values1AdditionalData);

$valuesArray []= $values1;
$requestRequestBody->setValues($valuesArray);
$result =  $graphClient->groupsById('group-id')->settings()->post($requestRequestBody);


```