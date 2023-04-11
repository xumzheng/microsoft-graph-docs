---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAllowedCombinationsPostRequestBody()
request_body.AllowedCombinations([request_body.AuthenticationMethodModes(AuthenticationMethodModes('password, voice'))
])



request_configuration = UpdateAllowedCombinationsRequestBuilderPostRequestConfiguration(
)


result = await client.policies.authenticationStrengthPolicies_by_id('authenticationStrengthPolicy-id').updateAllowedCombinations.post(request_body = request_body)


```