---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UpdateRecordingStatusPostRequestBody();
$requestBody->setClientContext('clientContext-value');

$requestBody->setStatus(new RecordingStatus('notrecording | recording | failed'));



$requestResult = $graphServiceClient->communications()->callsById('call-id')->updateRecordingStatus()->post($requestBody);


```