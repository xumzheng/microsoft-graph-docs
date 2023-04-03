---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationCategory();
requestBody.setDisplayName('Quizzes');



result = awaitclient.education().classesById('educationClass-id').assignmentCategories().post(requestBody);


```