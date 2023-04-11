---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationMethodConfiguration()
request_body.@odatatype = '#microsoft.graph.smsAuthenticationMethodConfiguration'

request_body.id = 'Sms'

request_body.State(AuthenticationMethodState('enabled'))



request_configuration = AuthenticationMethodConfigurationRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.authenticationMethodsPolicy.authenticationMethodConfigurations_by_id('authenticationMethodConfiguration-id').patch(request_body = request_body)


```