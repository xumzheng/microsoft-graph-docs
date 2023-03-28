---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new B2xIdentityUserFlow();
$requestBody.setId('Partner');

$requestBody.setUserFlowType(new UserFlowType('signuporsignin'));

$requestBody.setUserFlowTypeVersion(1);



$requestResult = $graphServiceClient.identity().b2xUserFlows().post($requestBody);


```