---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PersonAnnotation();
requestBody.setAllowedAudiences(AllowedAudiences('organization'));



result = awaitclient.usersById('user-id').profile().notesById('personAnnotation-id').patch(requestBody);


```