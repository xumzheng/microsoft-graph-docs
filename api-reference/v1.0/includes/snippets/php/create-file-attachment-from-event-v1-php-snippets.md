---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Attachment();


$requestRequestBody->setName('menu.txt');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.fileAttachment',
	"contentBytes" => 'base64bWFjIGFuZCBjaGVlc2UgdG9kYXk=',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->eventsById('event-id')->attachments()->post($requestRequestBody);


```