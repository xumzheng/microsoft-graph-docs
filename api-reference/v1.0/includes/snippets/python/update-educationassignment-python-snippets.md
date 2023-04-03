---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationAssignment();
requestBody.setDisplayName('Reading and review test 09.03 #5');

instructions = EducationItemBody();
instructions.setContentType(BodyType('text'));

instructions.setContent('Read chapter 5 and write your review');


requestBody.setInstructions($instructions);
requestBody.setDueDateTime(DateTime('2021-09-10T00:00:00Z'));

requestBody.setAddedStudentAction(EducationAddedStudentAction('none'));



result = await client.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').patch(requestBody);


```