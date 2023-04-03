---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UpdateRecordingStatusPostRequestBody();
requestBody.setClientContext('clientContext-value');

requestBody.setStatus(RecordingStatus('notrecording | recording | failed'));



requestResult = graphServiceClient.communications().callsById('call-id').updateRecordingStatus().post(requestBody);


```