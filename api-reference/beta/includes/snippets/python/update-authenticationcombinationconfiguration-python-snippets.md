---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationCombinationConfiguration()
request_body.setAppliesToCombinations([request_body.setAuthenticationMethodModes(AuthenticationMethodModes('fido2'))
])



result = await client.identity.conditionalAccess.authenticationStrengths.policiesby_id('authenticationStrengthPolicy-id').combinationConfigurationsby_id('authenticationCombinationConfiguration-id').patch(request_body)


```