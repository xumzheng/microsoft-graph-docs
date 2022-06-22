---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AgreementFileLocalization();


$requestRequestBody->setFileName('Contoso ToU for guest users (French)');
$requestRequestBody->setLanguage('fr-FR');
$requestRequestBody->setIsDefault(False);
$requestRequestBody->setIsMajorVersion(False);
$requestRequestBody->setDisplayName('Contoso ToU for guest users (French)');

$fileData = new AgreementFileData();
$requestRequestBody->setFileData($fileData);


$fileData->setData(base64_decode("base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data")););

$result =  $graphClient->identityGovernance()->termsOfUse()->agreementsById('agreement-id')->files()->post($requestRequestBody);


```