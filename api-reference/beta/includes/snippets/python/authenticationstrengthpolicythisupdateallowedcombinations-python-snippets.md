---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UpdateAllowedCombinationsPostRequestBody();
requestBody.setAllowedCombinations([requestBody.setAuthenticationMethodModes(AuthenticationMethodModes('password, voice'));
]);



result = await client.policies().authenticationStrengthPoliciesById('authenticationStrengthPolicy-id').updateAllowedCombinations().post(requestBody);


```