---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = IdentityUserFlow();
request_body.setId('Pol1');

request_body.setUserFlowType(UserFlowType('signuporsignin'));

request_body.setUserFlowTypeVersion(1);



result = await client.identity().userFlows().post(request_body);


```