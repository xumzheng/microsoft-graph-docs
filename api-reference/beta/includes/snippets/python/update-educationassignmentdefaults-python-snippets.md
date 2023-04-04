---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationAssignmentDefaults();
request_body.setAddedStudentAction(EducationAddedStudentAction('assignifopen'));

request_body.setNotificationChannelUrl('https://graph.microsoft.com/beta/teams(\'acdefc6b-2dc6-4e71-b1e9-6d9810ab1793\')/channels(\'3da03fc4-8eac-4459-84fb-1422dc01f65e\')');



result = await client.education().classesById('educationClass-id').assignmentDefaults().patch(request_body);


```