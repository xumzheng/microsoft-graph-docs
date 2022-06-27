---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ValueRequestBody();


$valueArray = [];

$valuevalue1 = new Alert();

$valuevalue1AdditionalData = [
	"assignedTo" => 'String',
	"closedDateTime" => 'String (timestamp)',
	"comments" => ['String',],
"id" => 'String (identifier)',
"tags" => ['String',],
];
$valuevalue1->setAdditionalData($valuevalue1AdditionalData);

$valueArray []= $valuevalue1;
$requestRequestBody->setValue($valueArray);
$result =  $graphClient->security()->alerts()->updateAlerts()->post($requestRequestBody);


```