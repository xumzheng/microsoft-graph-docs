---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AuthenticationFlowsPolicy();
$selfServiceSignUp = new SelfServiceSignUpAuthenticationFlowConfiguration();
$selfServiceSignUp.setIsEnabled(true);


$requestBody.setSelfServiceSignUp($selfServiceSignUp);


$requestResult = $graphServiceClient.policies().authenticationFlowsPolicy().patch($requestBody);


```