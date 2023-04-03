---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TeamworkTag();
requestBody.setDisplayName('Finance');



result = await client.teamsById('team-id').tagsById('teamworkTag-id').patch(requestBody);


```