---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlow()
request_body.id = 'Pol1'

request_body.UserFlowType(UserFlowType('signuporsignin'))

request_body.user_flow_type_version = 1




result = await client.identity.userFlows.post(request_body = request_body)


```