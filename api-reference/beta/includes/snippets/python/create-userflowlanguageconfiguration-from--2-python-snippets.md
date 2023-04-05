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




await client.identity.b2cUserFlows._by_id('b2cIdentityUserFlow-id').languages._by_id('userFlowLanguageConfiguration-id').put(request_body)


```