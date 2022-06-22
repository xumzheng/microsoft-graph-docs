---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Attachment();


$requestRequestBody->setName('name-value');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#Microsoft.OutlookServices.ItemAttachment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->eventsById('event-id')->attachments()->post($requestRequestBody);


```