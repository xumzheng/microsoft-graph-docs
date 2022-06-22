---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoveryHoldPolicy();


$requestRequestBody->setDisplayname('My legalHold with sources');
$requestRequestBody->setDescription('Created from Graph API');
$requestRequestBody->setContentQuery('Bazooka');
$requestRequestBodyAdditionalData = [
	"userSources@odata.bind" =>  [
	],
	"siteSources@odata.bind" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->legalHolds()->post($requestRequestBody);


```