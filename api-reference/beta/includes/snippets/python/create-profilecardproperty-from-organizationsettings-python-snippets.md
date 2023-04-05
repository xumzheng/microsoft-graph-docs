---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProfileCardProperty()
request_body.setDirectoryPropertyName('CustomAttribute1')

annotationsProfileCardAnnotation1 = ProfileCardAnnotation()
annotationsProfileCardAnnotation1.setDisplayName('Cost Center')

localizationsDisplayNameLocalization1 = DisplayNameLocalization()
localizationsDisplayNameLocalization1.setLanguageTag('ru-RU')

localizationsDisplayNameLocalization1.setDisplayName('центр затрат')


localizationsArray []= localizationsDisplayNameLocalization1;
annotationsProfileCardAnnotation1.setLocalizations(localizationsArray)



annotationsArray []= annotationsProfileCardAnnotation1;
request_body.setAnnotations(annotationsArray)




result = await client.organizationby_id('organization-id').settings.profileCardProperties.post(request_body)


```