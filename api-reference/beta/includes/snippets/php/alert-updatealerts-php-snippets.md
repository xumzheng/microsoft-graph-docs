---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ValueRequestBody();


$valueArray = [];

$value1 = new Alert();

$value1AdditionalData = [
		"assignedTo" => 'String',
		"closedDateTime" => 'String (timestamp)',
		"comments" =>  [
'String',		],
		"id" => 'String (identifier)',
		"tags" =>  [
'String',		],
	];
$value1->setAdditionalData($value1AdditionalData);

$valueArray []= $value1;
$requestRequestBody->setValue($valueArray);
$result =  $graphClient->security()->alerts()->updateAlerts()->post($requestRequestBody);


```