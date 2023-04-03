---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = RegionalAndLanguageSettingsPutRequestBody();
additionalData = [
'defaultDisplayLanguage' => requestBody = DefaultDisplayLanguage();
		requestBody.setLocale('en-US');


requestBody.setDefaultDisplayLanguage($defaultDisplayLanguage);

'authoringLanguages' => authoringLanguages1 = ();
		authoringLanguages1.setLocale('fr-FR');


authoringLanguagesArray []= authoringLanguages1;
authoringLanguages2 = ();
		authoringLanguages2.setLocale('de-DE');


authoringLanguagesArray []= authoringLanguages2;
requestBody.setAuthoringLanguages(authoringLanguagesArray);


'defaultTranslationLanguage' => requestBody = DefaultTranslationLanguage();
	requestBody.setLocale('en-US');


requestBody.setDefaultTranslationLanguage($defaultTranslationLanguage);

'defaultSpeechInputLanguage' => requestBody = DefaultSpeechInputLanguage();
	requestBody.setLocale('en-US');


requestBody.setDefaultSpeechInputLanguage($defaultSpeechInputLanguage);

'defaultRegionalFormat' => requestBody = DefaultRegionalFormat();
	requestBody.setLocale('en-GB');


requestBody.setDefaultRegionalFormat($defaultRegionalFormat);

'regionalFormatOverrides' => requestBody = RegionalFormatOverrides();
	requestBody.setCalendar('Gregorian Calendar');

	requestBody.setFirstDayOfWeek('Sunday');

	requestBody.setShortDateFormat('yyyy-MM-dd');

	requestBody.setLongDateFormat('dddd, MMMM d, yyyy');

	requestBody.setShortTimeFormat('HH:mm');

	requestBody.setLongTimeFormat('h:mm:ss tt');

	requestBody.setTimeZone('Pacific Standard Time');


requestBody.setRegionalFormatOverrides($regionalFormatOverrides);

'translationPreferences' => requestBody = TranslationPreferences();
	requestBody.setTranslationBehavior('Yes');

languageOverrides1 = ();
	languageOverrides1.setLanguageTag('fr');

	languageOverrides1.setTranslationBehavior('Yes');


languageOverridesArray []= languageOverrides1;
requestBody.setLanguageOverrides(languageOverridesArray);



requestBody.setTranslationPreferences($translationPreferences);

];
requestBody.setAdditionalData(additionalData);




graphServiceClient.me().settings().regionalAndLanguageSettings().put(requestBody);


```