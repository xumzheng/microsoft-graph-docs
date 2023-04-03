---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AuthenticationFlowsPolicy();
selfServiceSignUp = SelfServiceSignUpAuthenticationFlowConfiguration();
selfServiceSignUp.setIsEnabled(true);


requestBody.setSelfServiceSignUp($selfServiceSignUp);


result = await client.policies().authenticationFlowsPolicy().patch(requestBody);


```