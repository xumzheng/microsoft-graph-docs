---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RegionalAndLanguageSettings()
authoringLanguagesLocaleInfo1 = LocaleInfo()
authoringLanguagesLocaleInfo1.locale = 'en-US'


authoringLanguagesArray []= authoringLanguagesLocaleInfo1;
authoringLanguagesLocaleInfo2 = LocaleInfo()
authoringLanguagesLocaleInfo2.locale = 'es-MX'


authoringLanguagesArray []= authoringLanguagesLocaleInfo2;
request_body.authoringlanguages(authoringLanguagesArray)


defaultRegionalFormat = LocaleInfo()
defaultRegionalFormat.locale = 'en-US'


request_body.defaultRegionalFormat = defaultRegionalFormat


request_configuration = RegionalAndLanguageSettingsRequestBuilderPatchRequestConfiguration(
)


result = await client.me.settings.regionalAndLanguageSettings.patch(request_body = request_body)


```