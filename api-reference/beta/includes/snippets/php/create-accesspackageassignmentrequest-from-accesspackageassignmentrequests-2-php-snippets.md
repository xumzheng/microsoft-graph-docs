---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentRequest();


$requestRequestBody->setRequestType('UserAdd');

$accessPackageAssignment = new AccessPackageAssignment();
$requestRequestBody->setAccessPackageAssignment($accessPackageAssignment);


$accessPackageAssignment->setTargetId('46184453-e63b-4f20-86c2-c557ed5d5df9');
$accessPackageAssignment->setAssignmentPolicyId('2264bf65-76ba-417b-a27d-54d291f0cbc8');
$accessPackageAssignment->setAccessPackageId('a914b616-e04e-476b-aa37-91038f0b165b');

$answersArray = [];

$answers1 = new AccessPackageAnswer();


$answeredQuestion = new AccessPackageQuestion();
$answers1->setAnsweredQuestion($answeredQuestion);


$answeredQuestion->setId('A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF');
$answeredQuestionAdditionalData = [
	"@odata.type" => '#microsoft.graph.accessPackageMultipleChoiceQuestion',
];
$answeredQuestion->setAdditionalData($answeredQuestionAdditionalData);

$answers1AdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageAnswerString',
"value" => 'Arizona',
];
$answers1->setAdditionalData($answers1AdditionalData);

$answersArray []= $answers1;

$answers2 = new AccessPackageAnswer();


$answeredQuestion = new AccessPackageQuestion();
$answers2->setAnsweredQuestion($answeredQuestion);


$answeredQuestion->setId('AA615EE9-D9D8-4C03-BE91-BEE37106DEDA');
$answeredQuestionAdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageTextInputQuestion',
];
$answeredQuestion->setAdditionalData($answeredQuestionAdditionalData);

$answers2AdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageAnswerString',
"value" => 'Need access to marketing campaign material',
];
$answers2->setAdditionalData($answers2AdditionalData);

$answersArray []= $answers2;
$requestRequestBody->setAnswers($answersArray);
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentRequests()->post($requestRequestBody);


```