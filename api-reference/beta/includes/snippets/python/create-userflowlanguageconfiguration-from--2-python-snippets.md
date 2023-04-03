---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Language();
additionalData = [
'isEnabled' => false,
];
requestBody.setAdditionalData(additionalData);




awaitclient.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').languagesById('userFlowLanguageConfiguration-id').put(requestBody);


```