---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AppManagementPolicy();
$requestBody->setIsEnabled(false);



$requestResult = $graphServiceClient->policies()->appManagementPoliciesById('appManagementPolicy-id')->patch($requestBody);


```