---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProfileCardProperty()
request_body.directoryPropertyName = 'CustomAttribute1'

annotations_profile_card_annotation1 = ProfileCardAnnotation()
annotationsProfileCardAnnotation1.displayName = 'Cost Center'

localizations_display_name_localization1 = DisplayNameLocalization()
localizationsDisplayNameLocalization1.languageTag = 'ru-RU'

localizationsDisplayNameLocalization1.displayName = 'центр затрат'


localizationsArray []= localizationsDisplayNameLocalization1;
annotationsProfileCardAnnotation1.localizations(localizationsArray)



annotationsArray []= annotationsProfileCardAnnotation1;
request_body.annotations(annotationsArray)





result = await client.organization_by_id('organization-id').settings.profileCardProperties.post(request_body = request_body)


```