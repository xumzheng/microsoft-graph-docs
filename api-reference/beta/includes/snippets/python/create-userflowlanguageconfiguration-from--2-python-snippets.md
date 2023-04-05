---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Language()
additionalData = [
'isEnabled' => false,
];
request_body.setAdditionalData(additionalData)




await client.identity_b2cUserFlowsby_id('b2cIdentityUserFlow-id')_languagesby_id('userFlowLanguageConfiguration-id').put(request_body)


```