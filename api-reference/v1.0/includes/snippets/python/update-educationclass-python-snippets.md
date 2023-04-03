---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EducationClass();
requestBody.setDescription('History - World History 1');

requestBody.setDisplayName('World History Level 1');



requestResult = graphServiceClient.education().classesById('educationClass-id').patch(requestBody);


```