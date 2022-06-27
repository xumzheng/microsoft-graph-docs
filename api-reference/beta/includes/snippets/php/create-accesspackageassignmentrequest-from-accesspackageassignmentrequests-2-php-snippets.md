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

$answersanswers1 = new AccessPackageAnswer();


$answeredQuestion = new AccessPackageQuestion();
$answersanswers1->setAnsweredQuestion($answeredQuestion);


$answeredQuestion->setId('A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF');
$answeredQuestionAdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageMultipleChoiceQuestion',
];
$answeredQuestion->setAdditionalData($answeredQuestionAdditionalData);

$answersanswers1AdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageAnswerString',
"value" => 'Arizona',
];
$answersanswers1->setAdditionalData($answersanswers1AdditionalData);

$answersArray []= $answersanswers1;

$answersanswers2 = new AccessPackageAnswer();


$answeredQuestion = new AccessPackageQuestion();
$answersanswers2->setAnsweredQuestion($answeredQuestion);


$answeredQuestion->setId('AA615EE9-D9D8-4C03-BE91-BEE37106DEDA');
$answeredQuestionAdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageTextInputQuestion',
];
$answeredQuestion->setAdditionalData($answeredQuestionAdditionalData);

$answersanswers2AdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageAnswerString',
"value" => 'Need access to marketing campaign material',
];
$answersanswers2->setAdditionalData($answersanswers2AdditionalData);

$answersArray []= $answersanswers2;
$requestRequestBody->setAnswers($answersArray);
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentRequests()->post($requestRequestBody);


```