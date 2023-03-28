---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Incident();
$requestBody.setClassification(new AlertClassification('truepositive'));

$requestBody.setDetermination(new AlertDetermination('multistagedattack'));

$requestBody.setCustomTags(['Demo', ]);



$requestResult = $graphServiceClient.security().incidentsById('incident-id').patch($requestBody);


```