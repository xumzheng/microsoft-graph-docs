---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationCombinationConfiguration();
requestBody.setAppliesToCombinations([requestBody.setAuthenticationMethodModes(AuthenticationMethodModes('fido2'));
]);



result = awaitclient.identity().conditionalAccess().authenticationStrengths().policiesById('authenticationStrengthPolicy-id').combinationConfigurationsById('authenticationCombinationConfiguration-id').patch(requestBody);


```