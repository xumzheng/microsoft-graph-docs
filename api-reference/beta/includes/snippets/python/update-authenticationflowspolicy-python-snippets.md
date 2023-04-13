---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationFlowsPolicy()
self_service_sign_up = SelfServiceSignUpAuthenticationFlowConfiguration()
selfServiceSignUp.is_enabled = True


request_body.self_service_sign_up = selfServiceSignUp



result = await client.policies.authenticationFlowsPolicy.patch(request_body = request_body)


```