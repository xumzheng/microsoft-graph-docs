---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Alert();
$requestBody->setAssignedTo('secAdmin@contoso.onmicrosoft.com');

$requestBody->setClassification(new AlertClassification('truepositive'));

$requestBody->setDetermination(new AlertDetermination('malware'));

$requestBody->setStatus(new AlertStatus('inprogress'));



$requestResult = $graphServiceClient->security()->alerts_v2ById('alert-id')->patch($requestBody);


```