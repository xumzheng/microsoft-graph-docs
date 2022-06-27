---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RegionalAndLanguageSettings();


$authoringLanguagesArray = [];

$authoringLanguagesauthoringLanguages1 = new LocaleInfo();

$authoringLanguagesauthoringLanguages1->setLocale('en-US');

$authoringLanguagesArray []= $authoringLanguagesauthoringLanguages1;

$authoringLanguagesauthoringLanguages2 = new LocaleInfo();

$authoringLanguagesauthoringLanguages2->setLocale('es-MX');

$authoringLanguagesArray []= $authoringLanguagesauthoringLanguages2;
$requestRequestBody->setAuthoringLanguages($authoringLanguagesArray);

$defaultRegionalFormat = new LocaleInfo();
$requestRequestBody->setDefaultRegionalFormat($defaultRegionalFormat);


$defaultRegionalFormat->setLocale('en-US');

$result =  $graphClient->me()->settings()->regionalAndLanguageSettings()->patch($requestRequestBody);


```