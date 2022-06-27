---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ProfileCardProperty();


$requestRequestBody->setDirectoryPropertyName('CustomAttribute1');
$annotationsArray = [];

$annotationsannotations1 = new ProfileCardAnnotation();

$annotationsannotations1->setDisplayName('Cost Center');
$localizationsArray = [];

$localizationslocalizations1 = new DisplayNameLocalization();

$localizationslocalizations1->setLanguageTag('ru-RU');
$localizationslocalizations1->setDisplayName('центр затрат');

$localizationsArray []= $localizationslocalizations1;
$annotationsannotations1->setLocalizations($localizationsArray);

$annotationsArray []= $annotationsannotations1;
$requestRequestBody->setAnnotations($annotationsArray);
$result =  $graphClient->organizationById('organization-id')->settings()->profileCardProperties()->post($requestRequestBody);


```