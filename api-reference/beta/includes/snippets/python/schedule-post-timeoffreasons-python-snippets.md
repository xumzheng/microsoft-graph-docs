---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TimeOffReason();
$requestBody->setDisplayName('Vacation');

$requestBody->setIconType(new TimeOffReasonIconType('plane'));

$requestBody->setIsActive(true);



$requestResult = $graphServiceClient->teamsById('team-id')->schedule()->timeOffReasons()->post($requestBody);


```