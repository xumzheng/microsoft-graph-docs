---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationClass();
requestBody.setDescription('History - World History 1');

requestBody.setDisplayName('World History Level 1');



result = awaitclient.education().classesById('educationClass-id').patch(requestBody);


```