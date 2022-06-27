---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Attachment();


$requestRequestBody->setName('smile');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.fileAttachment',
	"contentBytes" => 'a0b1c76de9f7=',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->messagesById('message-id')->attachments()->post($requestRequestBody);


```