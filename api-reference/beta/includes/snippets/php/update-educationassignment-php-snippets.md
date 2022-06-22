---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationAssignment();


$requestRequestBody->setDisplayName('Reading and review test 09.03 #5');

$instructions = new EducationItemBody();
$requestRequestBody->setInstructions($instructions);


$instructions->setContentType(new BodyType('text'));
$instructions->setContent('Read chapter 5 and write your review');

$requestRequestBody->setDueDateTime(new DateTime("2021-09-10T00:00:00Z"));
$requestRequestBody->setAddedStudentAction(new EducationAddedStudentAction('none'));
$requestRequestBody->setAddToCalendarAction(new EducationAddToCalendarOptions('studentsAndPublisher'));
$result =  $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->patch($requestRequestBody);


```