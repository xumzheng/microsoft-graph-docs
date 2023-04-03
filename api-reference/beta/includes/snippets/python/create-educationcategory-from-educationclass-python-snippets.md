---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationCategory();
requestBody.setDisplayName('Quizzes');



result = await client.education().classesById('educationClass-id').assignmentCategories().post(requestBody);


```