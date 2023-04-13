---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = $valuePutRequestBody()
additionalData = [
'LocalizedStrings' => localized_strings1 = ()
		localizedStrings1.elementType = 'UxElement'

		localizedStrings1.elementId=null

		localizedStrings1.stringId = 'alert_message'

		localizedStrings1.override = True

		localizedStrings1.value = 'Are you sure that you want to cancel entering your information?'


localizedStringsArray []= localizedStrings1;
request_body.localizedstrings(localizedStringsArray)


];
request_body.additionaldata(additionalData)





await client.identity.b2xUserFlows_by_id('b2xIdentityUserFlow-id').languages_by_id('userFlowLanguageConfiguration-id').overridesPages_by_id('userFlowLanguagePage-id').content.put(request_body = request_body)


```