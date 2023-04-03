---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TeamsAppSettings();
requestBody.set@odatatype('#microsoft.graph.teamsAppSettings');

requestBody.setAllowUserRequestsForAppAccess(true);



requestResult = graphServiceClient.teamwork().teamsAppSettings().patch(requestBody);


```