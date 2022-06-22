---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ProfileCardProperty();


$requestRequestBody->setDirectoryPropertyName('CustomAttribute1');
$annotationsArray = [];

$annotations1 = new ProfileCardAnnotation();

$annotations1->setDisplayName('Cost Center');
$localizationsArray = [];

$localizations1 = new DisplayNameLocalization();

$localizations1->setLanguageTag('ru-RU');
$localizations1->setDisplayName('центр затрат');

$localizationsArray []= $localizations1;
$annotations1->setLocalizations($localizationsArray);

$annotationsArray []= $annotations1;
$requestRequestBody->setAnnotations($annotationsArray);
$result =  $graphClient->organizationById('organization-id')->settings()->profileCardProperties()->post($requestRequestBody);


```