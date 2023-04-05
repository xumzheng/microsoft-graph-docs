---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateRecordingStatusPostRequestBody()
request_body.setClientContext('clientContext-value')

request_body.setStatus(RecordingStatus('notrecording | recording | failed'))



result = await client.communications.calls_by_id('call-id').updateRecordingStatus.post(request_body)


```