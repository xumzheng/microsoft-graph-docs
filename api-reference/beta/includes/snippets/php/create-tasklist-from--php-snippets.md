---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BaseTaskList();


$requestRequestBody->setDisplayName('Shopping list');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.taskList',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->tasks()->lists()->post($requestRequestBody);


```