---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = B2cIdentityUserFlow();
requestBody.setIsLanguageCustomizationEnabled(true);

requestBody.setDefaultLanguageTag('en');



result = await client.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').patch(requestBody);


```