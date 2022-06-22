---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationAssignmentDefaults();


$requestRequestBody->setAddedStudentAction(new EducationAddedStudentAction('assignIfOpen'));
$requestRequestBody->setAddToCalendarAction(new EducationAddToCalendarOptions('studentsAndTeamOwners'));
$requestRequestBody->setNotificationChannelUrl('https://graph.microsoft.com/beta/teams(\'id\')/channels(\'id\')');
$result =  $graphClient->education()->classesById('educationClass-id')->assignmentDefaults()->patch($requestRequestBody);


```