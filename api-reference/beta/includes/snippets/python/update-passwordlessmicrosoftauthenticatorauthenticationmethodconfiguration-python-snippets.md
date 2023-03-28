---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AuthenticationMethodConfiguration();
$requestBody.set@odatatype('#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration');

$requestBody.setState(new AuthenticationMethodState('enabled'));



$requestResult = $graphServiceClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurationsById('authenticationMethodConfiguration-id').patch($requestBody);


```