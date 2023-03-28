---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AuthenticationCombinationConfiguration();
$requestBody.setAppliesToCombinations([$requestBody.setAuthenticationMethodModes(new AuthenticationMethodModes('fido2'));
]);



$requestResult = $graphServiceClient.identity().conditionalAccess().authenticationStrengths().policiesById('authenticationStrengthPolicy-id').combinationConfigurationsById('authenticationCombinationConfiguration-id').patch($requestBody);


```