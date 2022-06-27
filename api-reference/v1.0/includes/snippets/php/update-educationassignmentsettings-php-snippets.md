---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationAssignmentSettings();


$requestRequestBody->setSubmissionAnimationDisabled(True);
$result =  $graphClient->education()->classesById('educationClass-id')->assignmentSettings()->patch($requestRequestBody);


```