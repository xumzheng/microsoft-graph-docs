---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProfileCardProperty()
annotations_profile_card_annotation1 = ProfileCardAnnotation()
localizations_display_name_localization1 = DisplayNameLocalization()
localizationsDisplayNameLocalization1.languageTag = 'no-NB'

localizationsDisplayNameLocalization1.displayName = 'Kostnads Senter'


localizationsArray []= localizationsDisplayNameLocalization1;
annotationsProfileCardAnnotation1.localizations(localizationsArray)



annotationsArray []= annotationsProfileCardAnnotation1;
request_body.annotations(annotationsArray)





result = await client.organization_by_id('organization-id').settings.profileCardProperties_by_id('profileCardProperty-id').patch(request_body = request_body)


```