---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Attachment();


$requestRequestBody->setName('name-value');
$requestRequestBody->setContentType('contentType-value');
$requestRequestBody->setIsInline(False);
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#Microsoft.OutlookServices.FileAttachment',
	"contentLocation" => 'contentLocation-value',
	"contentBytes" => 'contentBytes-value',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->messagesById('message-id')->attachments()->post($requestRequestBody);


```