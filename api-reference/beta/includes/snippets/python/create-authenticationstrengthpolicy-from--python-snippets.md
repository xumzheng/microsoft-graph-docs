---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationStrengthPolicy();
requestBody.set@odatatype('#microsoft.graph.authenticationStrengthPolicy');

requestBody.setDisplayName('Contoso authentication level');

requestBody.setDescription('The only authentication level allowed to access our secret apps');

requestBody.setAllowedCombinations([requestBody.setAuthenticationMethodModes(AuthenticationMethodModes('password, hardwareoath'));
requestBody.setAuthenticationMethodModes(AuthenticationMethodModes('password, sms'));
]);



result = awaitclient.policies().authenticationStrengthPolicies().post(requestBody);


```