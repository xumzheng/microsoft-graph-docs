---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TeamworkTag();
requestBody.setDisplayName('Finance');



result = awaitclient.teamsById('team-id').tagsById('teamworkTag-id').patch(requestBody);


```