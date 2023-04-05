---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProfileCardProperty()
annotationsProfileCardAnnotation1 = ProfileCardAnnotation()
localizationsDisplayNameLocalization1 = DisplayNameLocalization()
localizationsDisplayNameLocalization1.setLanguageTag('no-NB')

localizationsDisplayNameLocalization1.setDisplayName('Kostnads Senter')


localizationsArray []= localizationsDisplayNameLocalization1;
annotationsProfileCardAnnotation1.setLocalizations(localizationsArray)



annotationsArray []= annotationsProfileCardAnnotation1;
request_body.setAnnotations(annotationsArray)




result = await client.organization._by_id('organization-id').settings.profileCardProperties._by_id('profileCardProperty-id').patch(request_body)


```