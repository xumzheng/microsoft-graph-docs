---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RegionalAndLanguageSettingsPutRequestBody()
additionalData = [
'defaultDisplayLanguage' => request_body = DefaultDisplayLanguage()
		request_body.locale = 'en-US'


request_body.default_display_language = defaultDisplayLanguage

'authoringLanguages' => authoring_languages1 = ()
		authoringLanguages1.locale = 'fr-FR'


authoringLanguagesArray []= authoringLanguages1;
authoring_languages2 = ()
		authoringLanguages2.locale = 'de-DE'


authoringLanguagesArray []= authoringLanguages2;
request_body.authoringlanguages(authoringLanguagesArray)


'defaultTranslationLanguage' => request_body = DefaultTranslationLanguage()
	request_body.locale = 'en-US'


request_body.default_translation_language = defaultTranslationLanguage

'defaultSpeechInputLanguage' => request_body = DefaultSpeechInputLanguage()
	request_body.locale = 'en-US'


request_body.default_speech_input_language = defaultSpeechInputLanguage

'defaultRegionalFormat' => request_body = DefaultRegionalFormat()
	request_body.locale = 'en-GB'


request_body.default_regional_format = defaultRegionalFormat

'regionalFormatOverrides' => request_body = RegionalFormatOverrides()
	request_body.calendar = 'Gregorian Calendar'

	request_body.firstDayOfWeek = 'Sunday'

	request_body.shortDateFormat = 'yyyy-MM-dd'

	request_body.longDateFormat = 'dddd, MMMM d, yyyy'

	request_body.shortTimeFormat = 'HH:mm'

	request_body.longTimeFormat = 'h:mm:ss tt'

	request_body.timeZone = 'Pacific Standard Time'


request_body.regional_format_overrides = regionalFormatOverrides

'translationPreferences' => request_body = TranslationPreferences()
	request_body.translationBehavior = 'Yes'

language_overrides1 = ()
	languageOverrides1.languageTag = 'fr'

	languageOverrides1.translationBehavior = 'Yes'


languageOverridesArray []= languageOverrides1;
request_body.languageoverrides(languageOverridesArray)



request_body.translation_preferences = translationPreferences

];
request_body.additionaldata(additionalData)





await client.me.settings.regionalAndLanguageSettings.put(request_body = request_body)


```