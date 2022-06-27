---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Attachment();


$requestRequestBody->setName('Personal pictures');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.referenceAttachment',
	"sourceUrl" => 'https://contoso.com/personal/mario_contoso_net/Documents/Pics',
	"providerType" => 'oneDriveConsumer',
	"permission" => 'Edit',
	"isFolder" => 'True',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->eventsById('event-id')->attachments()->post($requestRequestBody);


```