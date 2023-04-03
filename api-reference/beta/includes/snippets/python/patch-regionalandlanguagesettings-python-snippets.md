---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RegionalAndLanguageSettings();
authoringLanguagesLocaleInfo1 = LocaleInfo();
authoringLanguagesLocaleInfo1.setLocale('en-US');


authoringLanguagesArray []= authoringLanguagesLocaleInfo1;
authoringLanguagesLocaleInfo2 = LocaleInfo();
authoringLanguagesLocaleInfo2.setLocale('es-MX');


authoringLanguagesArray []= authoringLanguagesLocaleInfo2;
requestBody.setAuthoringLanguages(authoringLanguagesArray);


defaultRegionalFormat = LocaleInfo();
defaultRegionalFormat.setLocale('en-US');


requestBody.setDefaultRegionalFormat($defaultRegionalFormat);


result = awaitclient.me().settings().regionalAndLanguageSettings().patch(requestBody);


```