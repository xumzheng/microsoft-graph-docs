---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = B2cIdentityUserFlow();
request_body.setId('Customer');

request_body.setUserFlowType(UserFlowType('signuporsignin'));

request_body.setUserFlowTypeVersion(3);



result = await client.identity.b2cUserFlows.post(request_body);


```