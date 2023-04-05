---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationCategory()
request_body.setDisplayName('Quizzes')



result = await client.education.classesby_id('educationClass-id').assignmentCategories.post(request_body)


```