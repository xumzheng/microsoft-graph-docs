---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationFlowsPolicy();
selfServiceSignUp = SelfServiceSignUpAuthenticationFlowConfiguration();
selfServiceSignUp.setIsEnabled(true);


requestBody.setSelfServiceSignUp($selfServiceSignUp);


requestResult = graphServiceClient.policies().authenticationFlowsPolicy().patch(requestBody);


```