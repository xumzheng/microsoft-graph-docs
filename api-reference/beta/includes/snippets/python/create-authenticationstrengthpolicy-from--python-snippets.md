---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationStrengthPolicy()
request_body.@odatatype = '#microsoft.graph.authenticationStrengthPolicy'

request_body.displayName = 'Contoso authentication level'

request_body.description = 'The only authentication level allowed to access our secret apps'

request_body.AllowedCombinations([request_body.AuthenticationMethodModes(AuthenticationMethodModes('password, hardwareoath'))
request_body.AuthenticationMethodModes(AuthenticationMethodModes('password, sms'))
])



request_configuration = AuthenticationStrengthPoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.policies.authenticationStrengthPolicies.post(request_body = request_body)


```