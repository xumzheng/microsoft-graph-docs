---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationCategory()
request_body.displayName = 'Quizzes'



request_configuration = AssignmentCategoriesRequestBuilderPostRequestConfiguration(
)


result = await client.education.classes_by_id('educationClass-id').assignmentCategories.post(request_body = request_body)


```