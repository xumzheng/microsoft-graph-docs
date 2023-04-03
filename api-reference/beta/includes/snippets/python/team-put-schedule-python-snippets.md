---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Schedule();
requestBody.setEnabled(true);

requestBody.setTimeZone('America/Chicago');



result = await client.teamsById('team-id').schedule().put(requestBody);


```