---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationMethodConfiguration()
request_body.@odatatype = '#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration'

request_body.State(AuthenticationMethodState('enabled'))




result = await client.policies.authenticationMethodsPolicy.authenticationMethodConfigurations_by_id('authenticationMethodConfiguration-id').patch(request_body = request_body)


```