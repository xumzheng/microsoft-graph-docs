---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = $valuePutRequestBody()
additionalData = [
'LocalizedStrings' => localizedStrings1 = ()
		localizedStrings1.elementType = 'UxElement'

		localizedStrings1.elementId=null

		localizedStrings1.stringId = 'alert_message'

		localizedStrings1.override = true

		localizedStrings1.value = 'Are you sure that you want to cancel your selection?'


localizedStringsArray []= localizedStrings1;
request_body.localizedstrings(localizedStringsArray)


];
request_body.additionaldata(additionalData)




request_configuration = ContentRequestBuilderPutRequestConfiguration(
)


await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').languages_by_id('userFlowLanguageConfiguration-id').overridesPages_by_id('userFlowLanguagePage-id').content.put(request_body = request_body)


```