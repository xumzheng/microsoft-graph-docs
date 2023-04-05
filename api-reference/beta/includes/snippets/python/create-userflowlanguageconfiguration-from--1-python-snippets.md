---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Language()
additionalData = [
'id' => 'es-ES', 
'isEnabled' => true,
];
request_body.setAdditionalData(additionalData)




await client.identity.b2cUserFlowsby_id('b2cIdentityUserFlow-id').languagesby_id('userFlowLanguageConfiguration-id').put(request_body)


```