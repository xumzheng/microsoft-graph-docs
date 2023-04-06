---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationCombinationConfiguration()
request_body.setAppliesToCombinations([request_body.setAuthenticationMethodModes(AuthenticationMethodModes('fido2'))
])


request_config = AuthenticationCombinationConfigurationRequestBuilderPatchRequestConfiguration(
request_config = AuthenticationCombinationConfigurationRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identity.conditionalAccess.authenticationStrengths.policies_by_id('authenticationStrengthPolicy-id').combinationConfigurations_by_id('authenticationCombinationConfiguration-id').patch(request_body, headers=)


```