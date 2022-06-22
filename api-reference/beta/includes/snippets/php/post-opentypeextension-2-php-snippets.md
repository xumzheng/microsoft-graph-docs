---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Extension();


$requestRequestBodyAdditionalData = [
	"@odata.type" => 'microsoft.graph.openTypeExtension',
	"extensionName" => 'Com.Contoso.Referral',
	"companyName" => 'Wingtip Toys',
	"dealValue" => 500050,
	"expirationDate" => '2015-12-03T10:00:00.000Z',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->me()->messagesById('message-id')->extensions()->post($requestRequestBody);


```