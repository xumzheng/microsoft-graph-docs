---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationMethodConfiguration()
request_body.set@odatatype('#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration')

request_body.setState(AuthenticationMethodState('string'))



result = await client.policies.authenticationMethodsPolicy.authenticationMethodConfigurationsById('authenticationMethodConfiguration-id').patch(request_body)


```