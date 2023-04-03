---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ProfileCardProperty();
annotationsProfileCardAnnotation1 = ProfileCardAnnotation();
localizationsDisplayNameLocalization1 = DisplayNameLocalization();
localizationsDisplayNameLocalization1.setLanguageTag('no-NB');

localizationsDisplayNameLocalization1.setDisplayName('Kostnads Senter');


localizationsArray []= localizationsDisplayNameLocalization1;
annotationsProfileCardAnnotation1.setLocalizations(localizationsArray);



annotationsArray []= annotationsProfileCardAnnotation1;
requestBody.setAnnotations(annotationsArray);




result = awaitclient.organizationById('organization-id').settings().profileCardPropertiesById('profileCardProperty-id').patch(requestBody);


```