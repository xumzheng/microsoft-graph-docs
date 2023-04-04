---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationAssignmentSettings();
request_body.setSubmissionAnimationDisabled(true);



result = await client.education.classesById('educationClass-id').assignmentSettings.patch(request_body);


```