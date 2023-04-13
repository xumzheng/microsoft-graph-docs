---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2xIdentityUserFlow()
request_body.id = 'Partner'

request_body.UserFlowType(UserFlowType('signuporsignin'))

request_body.user_flow_type_version = 1




result = await client.identity.b2xUserFlows.post(request_body = request_body)


```