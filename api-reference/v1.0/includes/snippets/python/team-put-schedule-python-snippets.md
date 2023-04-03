---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Schedule();
requestBody.setEnabled(true);

requestBody.setTimeZone('America/Chicago');



requestResult = graphServiceClient.teamsById('team-id').schedule().put(requestBody);


```