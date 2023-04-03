---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SharePostRequestBody();
requestBody.setNotifyTeam(true);

requestBody.setStartDateTime(DateTime('2018-10-08T00:00:00.000Z'));

requestBody.setEndDateTime(DateTime('2018-10-15T00:00:00.000Z'));



graphServiceClient.teamsById('team-id').schedule().share().post(requestBody);


```