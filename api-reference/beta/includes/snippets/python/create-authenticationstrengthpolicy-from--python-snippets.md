---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AuthenticationStrengthPolicy();
$requestBody->set@odatatype('#microsoft.graph.authenticationStrengthPolicy');

$requestBody->setDisplayName('Contoso authentication level');

$requestBody->setDescription('The only authentication level allowed to access our secret apps');

$requestBody->setAllowedCombinations([$requestBody->setAuthenticationMethodModes(new AuthenticationMethodModes('password, hardwareoath'));
$requestBody->setAuthenticationMethodModes(new AuthenticationMethodModes('password, sms'));
]);



$requestResult = $graphServiceClient->policies()->authenticationStrengthPolicies()->post($requestBody);


```