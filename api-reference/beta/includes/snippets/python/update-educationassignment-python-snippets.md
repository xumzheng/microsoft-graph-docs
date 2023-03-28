---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EducationAssignment();
$requestBody.setDisplayName('Reading and review test 09.03 #5');

$instructions = new EducationItemBody();
$instructions.setContentType(new BodyType('text'));

$instructions.setContent('Read chapter 5 and write your review');


$requestBody.setInstructions($instructions);
$requestBody.setDueDateTime(new DateTime('2021-09-10T00:00:00Z'));

$requestBody.setAddedStudentAction(new EducationAddedStudentAction('none'));

$requestBody.setAddToCalendarAction(new EducationAddToCalendarOptions('studentsandpublisher'));



$requestResult = $graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').patch($requestBody);


```