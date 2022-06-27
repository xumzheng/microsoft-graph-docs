---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Agreement();


$requestRequestBody->setDisplayName('Contoso ToU for guest users');
$requestRequestBody->setIsViewingBeforeAcceptanceRequired(True);
$filesArray = [];

$filesfiles1 = new AgreementFileLocalization();

$filesfiles1AdditionalData = [
	"fileName" => 'TOU.pdf',
	"language" => 'en',
	"isDefault" => True,
];
$filesfiles1->setAdditionalData($filesfiles1AdditionalData);

$filesArray []= $filesfiles1;
$requestRequestBody->setFiles($filesArray);
$result =  $graphClient->identityGovernance()->termsOfUse()->agreements()->post($requestRequestBody);


```