---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignment()
request_body.dueDateTime = DateTime('2022-09-16T00:00:00Z')

request_body.displayName = 'Reading test 09.14'

instructions = EducationItemBody()
instructions.ContentType(BodyType('text'))

instructions.content = 'Read chapter 4'


request_body.instructions = instructions
grading = EducationAssignmentGradeType()
grading.@odatatype = '#microsoft.graph.educationAssignmentPointsGradeType'

additionalData = [
'maxPoints' => 50,
];
grading.additionaldata(additionalData)



request_body.grading = grading
assign_to = EducationAssignmentRecipient()
assignTo.@odatatype = '#microsoft.graph.educationAssignmentClassRecipient'


request_body.assign_to = assignTo
request_body.Status(EducationAssignmentStatus('draft'))

request_body.allow_students_to_add_resources_to_submission = True




result = await client.education.classes_by_id('educationClass-id').assignments.post(request_body = request_body)


```