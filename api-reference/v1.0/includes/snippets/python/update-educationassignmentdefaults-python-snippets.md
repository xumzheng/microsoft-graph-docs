---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationAssignmentDefaults();
requestBody.setAddedStudentAction(EducationAddedStudentAction('assignifopen'));

requestBody.setNotificationChannelUrl('https://graph.microsoft.com/beta/teams(\'acdefc6b-2dc6-4e71-b1e9-6d9810ab1793\')/channels(\'3da03fc4-8eac-4459-84fb-1422dc01f65e\')');



result = awaitclient.education().classesById('educationClass-id').assignmentDefaults().patch(requestBody);


```