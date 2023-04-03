---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationClass();
requestBody.setDescription('History - World History 1');

requestBody.setDisplayName('World History Level 1');



result = await client.education().classesById('educationClass-id').patch(requestBody);


```