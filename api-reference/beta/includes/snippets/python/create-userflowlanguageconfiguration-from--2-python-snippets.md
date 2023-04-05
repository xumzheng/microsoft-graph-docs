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




await client.identity.b2cUserFlowsById('b2cIdentityUserFlow-id').languagesById('userFlowLanguageConfiguration-id').put(request_body)


```