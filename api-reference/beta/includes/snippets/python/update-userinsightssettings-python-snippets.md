---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UserInsightsSettings();
$requestBody.setIsEnabled(false);



$requestResult = $graphServiceClient.usersById('user-id').settings().itemInsights().patch($requestBody);


```