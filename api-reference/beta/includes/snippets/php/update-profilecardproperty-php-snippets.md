---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ProfileCardProperty();


$annotationsArray = [];

$annotations1 = new ProfileCardAnnotation();

$localizationsArray = [];

$localizations1 = new DisplayNameLocalization();

$localizations1->setLanguageTag('no-NB');
$localizations1->setDisplayName('Kostnads Senter');

$localizationsArray []= $localizations1;
$annotations1->setLocalizations($localizationsArray);

$annotationsArray []= $annotations1;
$requestRequestBody->setAnnotations($annotationsArray);
$result =  $graphClient->organizationById('organization-id')->settings()->profileCardPropertiesById('profileCardProperty-id')->patch($requestRequestBody);


```