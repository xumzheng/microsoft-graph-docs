---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UpdateAllowedCombinationsPostRequestBody();
requestBody.setAllowedCombinations([requestBody.setAuthenticationMethodModes(AuthenticationMethodModes('password, voice'));
]);



requestResult = graphServiceClient.policies().authenticationStrengthPoliciesById('authenticationStrengthPolicy-id').updateAllowedCombinations().post(requestBody);


```