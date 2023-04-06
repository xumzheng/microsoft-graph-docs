---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentDefaults()
request_body.setAddedStudentAction(EducationAddedStudentAction('assignifopen'))

request_body.setAddToCalendarAction(EducationAddToCalendarOptions('studentsandteamowners'))

request_body.setNotificationChannelUrl('https://graph.microsoft.com/beta/teams(\'id\')/channels(\'id\')')


request_config = AssignmentDefaultsRequestBuilderPatchRequestConfiguration(
request_config = AssignmentDefaultsRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.education.classes_by_id('educationClass-id').assignmentDefaults.patch(request_body, headers=)


```