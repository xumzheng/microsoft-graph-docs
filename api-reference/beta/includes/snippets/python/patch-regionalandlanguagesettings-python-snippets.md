---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RegionalAndLanguageSettings()
authoring_languages_locale_info1 = LocaleInfo()
authoringLanguagesLocaleInfo1.locale = 'en-US'


authoringLanguagesArray []= authoringLanguagesLocaleInfo1;
authoring_languages_locale_info2 = LocaleInfo()
authoringLanguagesLocaleInfo2.locale = 'es-MX'


authoringLanguagesArray []= authoringLanguagesLocaleInfo2;
request_body.authoringlanguages(authoringLanguagesArray)


default_regional_format = LocaleInfo()
defaultRegionalFormat.locale = 'en-US'


request_body.default_regional_format = defaultRegionalFormat



result = await client.me.settings.regionalAndLanguageSettings.patch(request_body = request_body)


```