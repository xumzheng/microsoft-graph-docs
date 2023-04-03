---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TeamsAppSettings();
requestBody.set@odatatype('#microsoft.graph.teamsAppSettings');

requestBody.setIsChatResourceSpecificConsentEnabled(true);



result = await client.teamwork().teamsAppSettings().patch(requestBody);


```