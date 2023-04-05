---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignment()
request_body.setDueDateTime(DateTime('2022-09-16T00:00:00Z'))

request_body.setDisplayName('Reading test 09.14 Beta')

instructions = EducationItemBody()
instructions.setContentType(BodyType('text'))

instructions.setContent('Read chapter 4')


request_body.setInstructions($instructions)
grading = EducationAssignmentGradeType()
grading.set@odatatype('#microsoft.graph.educationAssignmentPointsGradeType')

additionalData = [
'maxPoints' => 50,
];
grading.setAdditionalData(additionalData)



request_body.setGrading($grading)
assignTo = EducationAssignmentRecipient()
assignTo.set@odatatype('#microsoft.graph.educationAssignmentClassRecipient')


request_body.setAssignTo($assignTo)
request_body.setStatus(EducationAssignmentStatus('draft'))

request_body.setAllowStudentsToAddResourcesToSubmission(true)



result = await client.education.classesby_id('educationClass-id').assignments.post(request_body)


```