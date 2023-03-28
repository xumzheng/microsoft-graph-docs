---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityUserFlow();
$requestBody->setId('Pol1');

$requestBody->setUserFlowType(new UserFlowType('signuporsignin'));

$requestBody->setUserFlowTypeVersion(1);



$requestResult = $graphServiceClient->identity()->userFlows()->post($requestBody);


```