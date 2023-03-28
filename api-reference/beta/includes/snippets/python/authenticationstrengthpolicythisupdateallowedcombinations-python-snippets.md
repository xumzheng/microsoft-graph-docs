---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UpdateAllowedCombinationsPostRequestBody();
$requestBody.setAllowedCombinations([$requestBody.setAuthenticationMethodModes(new AuthenticationMethodModes('password, voice'));
]);



$requestResult = $graphServiceClient.policies().authenticationStrengthPoliciesById('authenticationStrengthPolicy-id').updateAllowedCombinations().post($requestBody);


```