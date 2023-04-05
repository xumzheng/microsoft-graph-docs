---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = $valuePutRequestBody()
additionalData = [
'LocalizedStrings' => localizedStrings1 = ()
		localizedStrings1.setElementType('UxElement')

		localizedStrings1.setElementId(null)

		localizedStrings1.setStringId('alert_message')

		localizedStrings1.setOverride(true)

		localizedStrings1.setValue('Are you sure that you want to cancel entering your information?')


localizedStringsArray []= localizedStrings1;
request_body.setLocalizedStrings(localizedStringsArray)


];
request_body.setAdditionalData(additionalData)




await client.identity.b2xUserFlowsby_id('b2xIdentityUserFlow-id').languagesby_id('userFlowLanguageConfiguration-id').overridesPagesby_id('userFlowLanguagePage-id').content.put(request_body)


```