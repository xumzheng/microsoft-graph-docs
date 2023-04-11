---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateRecordingStatusPostRequestBody()
request_body.clientContext = 'clientContext-value'

request_body.Status(RecordingStatus('notrecording | recording | failed'))



request_configuration = UpdateRecordingStatusRequestBuilderPostRequestConfiguration(
)


result = await client.communications.calls_by_id('call-id').updateRecordingStatus.post(request_body = request_body)


```