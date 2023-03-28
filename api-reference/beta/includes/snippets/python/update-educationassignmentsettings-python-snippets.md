---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EducationAssignmentSettings();
$requestBody.setSubmissionAnimationDisabled(true);



$requestResult = $graphServiceClient.education().classesById('educationClass-id').assignmentSettings().patch($requestBody);


```