---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RegionalAndLanguageSettings();


$authoringLanguagesArray = [];

$authoringLanguages1 = new LocaleInfo();

$authoringLanguages1->setLocale('en-US');

$authoringLanguagesArray []= $authoringLanguages1;

$authoringLanguages2 = new LocaleInfo();

$authoringLanguages2->setLocale('es-MX');

$authoringLanguagesArray []= $authoringLanguages2;
$requestRequestBody->setAuthoringLanguages($authoringLanguagesArray);

$defaultRegionalFormat = new LocaleInfo();
$requestRequestBody->setDefaultRegionalFormat($defaultRegionalFormat);


$defaultRegionalFormat->setLocale('en-US');

$result =  $graphClient->me()->settings()->regionalAndLanguageSettings()->patch($requestRequestBody);


```