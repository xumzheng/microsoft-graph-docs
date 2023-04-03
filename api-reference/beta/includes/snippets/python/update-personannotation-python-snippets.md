---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PersonAnnotation();
requestBody.setAllowedAudiences(AllowedAudiences('organization'));



result = await client.usersById('user-id').profile().notesById('personAnnotation-id').patch(requestBody);


```