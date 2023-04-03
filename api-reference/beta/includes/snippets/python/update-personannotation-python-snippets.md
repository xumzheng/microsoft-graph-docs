---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PersonAnnotation();
requestBody.setAllowedAudiences(AllowedAudiences('organization'));



requestResult = graphServiceClient.usersById('user-id').profile().notesById('personAnnotation-id').patch(requestBody);


```