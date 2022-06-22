---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationAssignmentDefaults();


$requestRequestBody->setAddedStudentAction(new EducationAddedStudentAction('assignIfOpen'));
$requestRequestBody->setNotificationChannelUrl('https://graph.microsoft.com/beta/teams(\'acdefc6b-2dc6-4e71-b1e9-6d9810ab1793\')/channels(\'3da03fc4-8eac-4459-84fb-1422dc01f65e\')');
$result =  $graphClient->education()->classesById('educationClass-id')->assignmentDefaults()->patch($requestRequestBody);


```