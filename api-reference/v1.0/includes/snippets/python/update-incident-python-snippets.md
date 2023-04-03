---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Incident();
requestBody.setClassification(AlertClassification('truepositive'));

requestBody.setDetermination(AlertDetermination('multistagedattack'));

requestBody.setCustomTags(['Demo', ]);



requestResult = graphServiceClient.security().incidentsById('incident-id').patch(requestBody);


```