---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new EducationOutcome();
$requestBody->set@odatatype('#microsoft.graph.educationFeedbackOutcome');

$additionalData = [
		'feedback' => $requestBody = new Feedback();
$text = new Text();
$		text->setContent('This is feedback for the assignment as a whole.');

$		text->setContentType('text');


$requestBody->setText($text);

$requestBody->setFeedback($feedback);

];
$requestBody->setAdditionalData($additionalData);




$result = $graphServiceClient->education()->classes()->byClasseId('educationClass-id')->assignments()->byAssignmentId('educationAssignment-id')->submissions()->bySubmissionId('educationSubmission-id')->outcomes()->byOutcomeId('educationOutcome-id')->patch($requestBody);


```