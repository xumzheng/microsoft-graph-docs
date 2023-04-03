---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UpdateAllowedCombinationsPostRequestBody();
requestBody.setAllowedCombinations([requestBody.setAuthenticationMethodModes(AuthenticationMethodModes('password, voice'));
]);



result = awaitclient.policies().authenticationStrengthPoliciesById('authenticationStrengthPolicy-id').updateAllowedCombinations().post(requestBody);


```