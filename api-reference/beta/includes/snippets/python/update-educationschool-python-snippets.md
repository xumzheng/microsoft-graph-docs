---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationSchool();
requestBody.setDisplayName('Fabrikam Arts High School');

requestBody.setDescription('Magnate school for the arts. Los Angeles School District');



result = awaitclient.education().schoolsById('educationSchool-id').patch(requestBody);


```