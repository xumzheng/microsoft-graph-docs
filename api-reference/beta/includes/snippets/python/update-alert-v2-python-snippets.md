---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Alert();
requestBody.setAssignedTo('secAdmin@contoso.onmicrosoft.com');

requestBody.setClassification(AlertClassification('truepositive'));

requestBody.setDetermination(AlertDetermination('malware'));

requestBody.setStatus(AlertStatus('inprogress'));



result = awaitclient.security().alerts_v2ById('alert-id').patch(requestBody);


```