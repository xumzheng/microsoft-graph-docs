---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = B2cIdentityUserFlow();
request_body.setIsLanguageCustomizationEnabled(true);

request_body.setDefaultLanguageTag('en');



result = await client.identity().b2cUserFlowsById('b2cIdentityUserFlow-id').patch(request_body);


```