---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Incident()
request_body.setClassification(AlertClassification('truepositive'))

request_body.setDetermination(AlertDetermination('multistagedattack'))

request_body.setCustomTags(['Demo', ])



result = await client.security.incidents_by_id('incident-id').patch(request_body)


```