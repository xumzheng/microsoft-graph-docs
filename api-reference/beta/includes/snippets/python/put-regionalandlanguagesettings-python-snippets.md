---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RegionalAndLanguageSettingsPutRequestBody()
additionalData = [
'defaultDisplayLanguage' => request_body = DefaultDisplayLanguage()
		request_body.setLocale('en-US')


request_body.setDefaultDisplayLanguage($defaultDisplayLanguage)

'authoringLanguages' => authoringLanguages1 = ()
		authoringLanguages1.setLocale('fr-FR')


authoringLanguagesArray []= authoringLanguages1;
authoringLanguages2 = ()
		authoringLanguages2.setLocale('de-DE')


authoringLanguagesArray []= authoringLanguages2;
request_body.setAuthoringLanguages(authoringLanguagesArray)


'defaultTranslationLanguage' => request_body = DefaultTranslationLanguage()
	request_body.setLocale('en-US')


request_body.setDefaultTranslationLanguage($defaultTranslationLanguage)

'defaultSpeechInputLanguage' => request_body = DefaultSpeechInputLanguage()
	request_body.setLocale('en-US')


request_body.setDefaultSpeechInputLanguage($defaultSpeechInputLanguage)

'defaultRegionalFormat' => request_body = DefaultRegionalFormat()
	request_body.setLocale('en-GB')


request_body.setDefaultRegionalFormat($defaultRegionalFormat)

'regionalFormatOverrides' => request_body = RegionalFormatOverrides()
	request_body.setCalendar('Gregorian Calendar')

	request_body.setFirstDayOfWeek('Sunday')

	request_body.setShortDateFormat('yyyy-MM-dd')

	request_body.setLongDateFormat('dddd, MMMM d, yyyy')

	request_body.setShortTimeFormat('HH:mm')

	request_body.setLongTimeFormat('h:mm:ss tt')

	request_body.setTimeZone('Pacific Standard Time')


request_body.setRegionalFormatOverrides($regionalFormatOverrides)

'translationPreferences' => request_body = TranslationPreferences()
	request_body.setTranslationBehavior('Yes')

languageOverrides1 = ()
	languageOverrides1.setLanguageTag('fr')

	languageOverrides1.setTranslationBehavior('Yes')


languageOverridesArray []= languageOverrides1;
request_body.setLanguageOverrides(languageOverridesArray)



request_body.setTranslationPreferences($translationPreferences)

];
request_body.setAdditionalData(additionalData)



request_config = RegionalAndLanguageSettingsRequestBuilderPutRequestConfiguration(
request_config = RegionalAndLanguageSettingsRequestBuilderPutRequestConfiguration(query_params=)


await client.me.settings.regionalAndLanguageSettings.put(request_body, headers=)


```