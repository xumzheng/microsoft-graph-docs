---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ProfileCardProperty();
$annotationsProfileCardAnnotation1 = new ProfileCardAnnotation();
$localizationsDisplayNameLocalization1 = new DisplayNameLocalization();
$localizationsDisplayNameLocalization1.setLanguageTag('no-NB');

$localizationsDisplayNameLocalization1.setDisplayName('Kostnads Senter');


$localizationsArray []= $localizationsDisplayNameLocalization1;
$annotationsProfileCardAnnotation1.setLocalizations($localizationsArray);



$annotationsArray []= $annotationsProfileCardAnnotation1;
$requestBody.setAnnotations($annotationsArray);




$requestResult = $graphServiceClient.organizationById('organization-id').settings().profileCardPropertiesById('profileCardProperty-id').patch($requestBody);


```