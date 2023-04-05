---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentSettings()
request_body.setSubmissionAnimationDisabled(true)



result = await client.education_classesby_id('educationClass-id')_assignmentSettings.patch(request_body)


```