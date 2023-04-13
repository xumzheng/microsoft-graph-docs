---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Alert()
request_body.assignedTo = 'secAdmin@contoso.onmicrosoft.com'

request_body.Classification(AlertClassification('truepositive'))

request_body.Determination(AlertDetermination('malware'))

request_body.Status(AlertStatus('inprogress'))




result = await client.security.alerts_v2_by_id('alert-id').patch(request_body = request_body)


```