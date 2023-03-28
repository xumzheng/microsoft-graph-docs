---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RegionalAndLanguageSettings();
$authoringLanguagesLocaleInfo1 = new LocaleInfo();
$authoringLanguagesLocaleInfo1->setLocale('en-US');


$authoringLanguagesArray []= $authoringLanguagesLocaleInfo1;
$authoringLanguagesLocaleInfo2 = new LocaleInfo();
$authoringLanguagesLocaleInfo2->setLocale('es-MX');


$authoringLanguagesArray []= $authoringLanguagesLocaleInfo2;
$requestBody->setAuthoringLanguages($authoringLanguagesArray);


$defaultRegionalFormat = new LocaleInfo();
$defaultRegionalFormat->setLocale('en-US');


$requestBody->setDefaultRegionalFormat($defaultRegionalFormat);


$requestResult = $graphServiceClient->me()->settings()->regionalAndLanguageSettings()->patch($requestBody);


```