---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Schedule();
requestBody.setEnabled(true);

requestBody.setTimeZone('America/Chicago');



result = awaitclient.teamsById('team-id').schedule().put(requestBody);


```