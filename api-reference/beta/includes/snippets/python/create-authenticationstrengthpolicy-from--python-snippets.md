---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationStrengthPolicy()
request_body.set@odatatype('#microsoft.graph.authenticationStrengthPolicy')

request_body.setDisplayName('Contoso authentication level')

request_body.setDescription('The only authentication level allowed to access our secret apps')

request_body.setAllowedCombinations([request_body.setAuthenticationMethodModes(AuthenticationMethodModes('password, hardwareoath'))
request_body.setAuthenticationMethodModes(AuthenticationMethodModes('password, sms'))
])


request_config = AuthenticationStrengthPoliciesRequestBuilderPostRequestConfiguration(
request_config = AuthenticationStrengthPoliciesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.policies.authenticationStrengthPolicies.post(request_body, headers=)


```