---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UpdateRecordingStatusPostRequestBody();
requestBody.setClientContext('clientContext-value');

requestBody.setStatus(RecordingStatus('notrecording | recording | failed'));



result = await client.communications().callsById('call-id').updateRecordingStatus().post(requestBody);


```