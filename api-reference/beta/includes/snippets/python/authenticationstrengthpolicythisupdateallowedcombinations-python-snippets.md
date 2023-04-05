---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAllowedCombinationsPostRequestBody()
request_body.setAllowedCombinations([request_body.setAuthenticationMethodModes(AuthenticationMethodModes('password, voice'))
])



result = await client.policies_authenticationStrengthPoliciesby_id('authenticationStrengthPolicy-id')_updateAllowedCombinations.post(request_body)


```