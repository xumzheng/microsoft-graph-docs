---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationFlowsPolicy()
selfServiceSignUp = SelfServiceSignUpAuthenticationFlowConfiguration()
selfServiceSignUp.isEnabled = true


request_body.selfServiceSignUp = selfServiceSignUp



result = await client.policies.authenticationFlowsPolicy.patch(request_body = request_body)


```