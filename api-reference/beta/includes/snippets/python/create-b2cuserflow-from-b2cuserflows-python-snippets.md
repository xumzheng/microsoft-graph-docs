---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = B2cIdentityUserFlow();
requestBody.setId('Customer');

requestBody.setUserFlowType(UserFlowType('signuporsignin'));

requestBody.setUserFlowTypeVersion(3);



requestResult = graphServiceClient.identity().b2cUserFlows().post(requestBody);


```