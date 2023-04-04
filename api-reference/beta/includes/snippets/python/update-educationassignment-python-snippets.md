---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationAssignment()
request_body.setDisplayName('Reading and review test 09.03 #5')

instructions = EducationItemBody()
instructions.setContentType(BodyType('text'))

instructions.setContent('Read chapter 5 and write your review')


request_body.setInstructions($instructions)
request_body.setDueDateTime(DateTime('2021-09-10T00:00:00Z'))

request_body.setAddedStudentAction(EducationAddedStudentAction('none'))

request_body.setAddToCalendarAction(EducationAddToCalendarOptions('studentsandpublisher'))



result = await client.education.classesById('educationClass-id').assignmentsById('educationAssignment-id').patch(request_body)


```