---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Attachment();


$requestRequestBody->setName('Holiday event');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.itemAttachment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->outlook()->tasksById('outlookTask-id')->attachments()->post($requestRequestBody);


```