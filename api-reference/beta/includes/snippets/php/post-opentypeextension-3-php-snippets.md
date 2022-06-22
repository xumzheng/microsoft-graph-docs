---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Extension();


$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.openTypeExtension',
	"extensionName" => 'Com.Contoso.Deal',
	"companyName" => 'Alpine Skis',
	"dealValue" => 1010100,
	"expirationDate" => '2015-07-03T13:04:00.000Z',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->groupsById('group-id')->eventsById('event-id')->extensions()->post($requestRequestBody);


```