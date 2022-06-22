---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Extension();


$requestRequestBodyAdditionalData = [
	"@odata.type" => 'Microsoft.OutlookServices.OpenTypeExtension',
	"extensionName" => 'Com.Contoso.Estimate',
	"companyName" => 'Contoso',
	"expirationDate" => '2016-07-30T11:00:00.000Z',
	"DealValue" => 1010100,
	"topPicks" =>  [
'Employees only','Add spouse or guest','Add family',	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->postsById('post-id')->extensionsById('extension-id')->patch($requestRequestBody);


```