---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Schedule();
$requestBody->setEnabled(true);

$requestBody->setTimeZone('America/Chicago');



$requestResult = $graphServiceClient->teamsById('team-id')->schedule()->put($requestBody);


```