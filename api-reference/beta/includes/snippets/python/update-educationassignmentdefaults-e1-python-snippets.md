---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentDefaults()
request_body.AddedStudentAction(EducationAddedStudentAction('assignifopen'))

request_body.AddToCalendarAction(EducationAddToCalendarOptions('studentsandteamowners'))

request_body.notificationChannelUrl = 'https://graph.microsoft.com/beta/teams(\'id\')/channels(\'id\')'




result = await client.education.classes_by_id('educationClass-id').assignmentDefaults.patch(request_body = request_body)


```