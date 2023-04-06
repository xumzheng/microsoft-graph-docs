---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationMethodConfiguration()
request_body.set@odatatype('#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration')

request_body.setState(AuthenticationMethodState('enabled'))


request_config = AuthenticationMethodConfigurationRequestBuilderPatchRequestConfiguration(
request_config = AuthenticationMethodConfigurationRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.policies.authenticationMethodsPolicy.authenticationMethodConfigurations_by_id('authenticationMethodConfiguration-id').patch(request_body, headers=)


```