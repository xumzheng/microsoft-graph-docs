---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationAssignment();
requestBody.setDueDateTime(DateTime('2022-09-16T00:00:00Z'));

requestBody.setDisplayName('Reading test 09.14 Beta');

instructions = EducationItemBody();
instructions.setContentType(BodyType('text'));

instructions.setContent('Read chapter 4');


requestBody.setInstructions($instructions);
grading = EducationAssignmentGradeType();
grading.set@odatatype('#microsoft.graph.educationAssignmentPointsGradeType');

additionalData = [
'maxPoints' => 50,
];
grading.setAdditionalData(additionalData);



requestBody.setGrading($grading);
assignTo = EducationAssignmentRecipient();
assignTo.set@odatatype('#microsoft.graph.educationAssignmentClassRecipient');


requestBody.setAssignTo($assignTo);
requestBody.setStatus(EducationAssignmentStatus('draft'));

requestBody.setAllowStudentsToAddResourcesToSubmission(true);



result = await client.education().classesById('educationClass-id').assignments().post(requestBody);


```