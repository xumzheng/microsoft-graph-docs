---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationAssignment();


$requestRequestBody->setDueDateTime(new DateTime("2021-09-07T00:00:00Z"));
$requestRequestBody->setDisplayName('Reading test 09.03 #4');

$instructions = new EducationItemBody();
$requestRequestBody->setInstructions($instructions);


$instructions->setContentType(new BodyType('text'));
$instructions->setContent('Read chapter 4');


$grading = new EducationAssignmentGradeType();
$requestRequestBody->setGrading($grading);


$gradingAdditionalData = [
"@odata.type" => '#microsoft.graph.educationAssignmentPointsGradeType',
"maxPoints" => 50,
];
$grading->setAdditionalData($gradingAdditionalData);


$assignTo = new EducationAssignmentRecipient();
$requestRequestBody->setAssignTo($assignTo);


$assignToAdditionalData = [
"@odata.type" => '#microsoft.graph.educationAssignmentClassRecipient',
];
$assignTo->setAdditionalData($assignToAdditionalData);

$requestRequestBody->setStatus(new EducationAssignmentStatus('draft'));
$requestRequestBody->setAllowStudentsToAddResourcesToSubmission(True);
$result =  $graphClient->education()->classesById('educationClass-id')->assignments()->post($requestRequestBody);


```