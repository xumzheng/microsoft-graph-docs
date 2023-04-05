---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Alert()
request_body.setAssignedTo('secAdmin@contoso.onmicrosoft.com')

request_body.setClassification(AlertClassification('truepositive'))

request_body.setDetermination(AlertDetermination('malware'))

request_body.setStatus(AlertStatus('inprogress'))



result = await client.security_alerts_v2by_id('alert-id').patch(request_body)


```