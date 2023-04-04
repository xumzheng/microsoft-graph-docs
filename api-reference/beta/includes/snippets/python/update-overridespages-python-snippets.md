---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = $valuePutRequestBody();
additionalData = [
'LocalizedStrings' => localizedStrings1 = ();
		localizedStrings1.setElementType('UxElement');

		localizedStrings1.setElementId(null);

		localizedStrings1.setStringId('alert_message');

		localizedStrings1.setOverride(true);

		localizedStrings1.setValue('Are you sure that you want to cancel your selection?');


localizedStringsArray []= localizedStrings1;
request_body.setLocalizedStrings(localizedStringsArray);


];
request_body.setAdditionalData(additionalData);




await client.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').languagesById('userFlowLanguageConfiguration-id').overridesPagesById('userFlowLanguagePage-id').value().put(request_body);


```