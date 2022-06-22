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

$files1 = new AgreementFileLocalization();

$files1AdditionalData = [
		"fileName" => 'TOU.pdf',
		"language" => 'en',
		"isDefault" => True,
	];
$files1->setAdditionalData($files1AdditionalData);

$filesArray []= $files1;
$requestRequestBody->setFiles($filesArray);
$result =  $graphClient->identityGovernance()->termsOfUse()->agreements()->post($requestRequestBody);


```