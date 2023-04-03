---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationFlowsPolicy();
selfServiceSignUp = SelfServiceSignUpAuthenticationFlowConfiguration();
selfServiceSignUp.setIsEnabled(true);


requestBody.setSelfServiceSignUp($selfServiceSignUp);


result = awaitclient.policies().authenticationFlowsPolicy().patch(requestBody);


```