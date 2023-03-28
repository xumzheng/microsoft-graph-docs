---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SecureScoreControlProfile();
$requestBody->setControlStateUpdates('controlStateUpdates-value');



$requestResult = $graphServiceClient->security()->secureScoreControlProfilesById('secureScoreControlProfile-id')->patch($requestBody);


```