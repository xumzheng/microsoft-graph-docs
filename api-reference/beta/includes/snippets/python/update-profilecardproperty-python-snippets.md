---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Profile_card_property()
annotations_profile_card_annotation1 = Profile_card_annotation()
localizations_display_name_localization1 = Display_name_localization()
localizations_display_name_localization1.language_tag = 'no-NB'

localizations_display_name_localization1.display_name = 'Kostnads Senter'


localizationsArray []= localizationsDisplayNameLocalization1;
annotations_profile_card_annotation1.localizations(localizationsArray)



annotationsArray []= annotationsProfileCardAnnotation1;
request_body.annotations(annotationsArray)





result = await client.organization.by_organization_id('organization-id').settings.profile_card_properties.by_profile_card_propertie_id('profileCardProperty-id').patch(request_body = request_body)


```