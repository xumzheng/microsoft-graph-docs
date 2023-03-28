---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AuthorizationPolicy();
$requestBody.setBlockMsolPowerShell(true);



$requestResult = $graphServiceClient.policies().authorizationPolicyById('authorizationPolicy-id').patch($requestBody);


```