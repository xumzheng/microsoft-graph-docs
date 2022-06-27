---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ProfileCardProperty();


$annotationsArray = [];

$annotationsannotations1 = new ProfileCardAnnotation();

$localizationsArray = [];

$localizationslocalizations1 = new DisplayNameLocalization();

$localizationslocalizations1->setLanguageTag('no-NB');
$localizationslocalizations1->setDisplayName('Kostnads Senter');

$localizationsArray []= $localizationslocalizations1;
$annotationsannotations1->setLocalizations($localizationsArray);

$annotationsArray []= $annotationsannotations1;
$requestRequestBody->setAnnotations($annotationsArray);
$result =  $graphClient->organizationById('organization-id')->settings()->profileCardPropertiesById('profileCardProperty-id')->patch($requestRequestBody);


```