---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = RegionalAndLanguageSettings();
authoringLanguagesLocaleInfo1 = LocaleInfo();
authoringLanguagesLocaleInfo1.setLocale('en-US');


authoringLanguagesArray []= authoringLanguagesLocaleInfo1;
authoringLanguagesLocaleInfo2 = LocaleInfo();
authoringLanguagesLocaleInfo2.setLocale('es-MX');


authoringLanguagesArray []= authoringLanguagesLocaleInfo2;
request_body.setAuthoringLanguages(authoringLanguagesArray);


defaultRegionalFormat = LocaleInfo();
defaultRegionalFormat.setLocale('en-US');


request_body.setDefaultRegionalFormat($defaultRegionalFormat);


result = await client.me().settings().regionalAndLanguageSettings().patch(request_body);


```