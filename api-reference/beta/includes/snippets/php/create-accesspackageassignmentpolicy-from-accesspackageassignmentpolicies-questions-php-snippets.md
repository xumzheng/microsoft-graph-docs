---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentPolicy();


$requestRequestBody->setAccessPackageId('b2eba9a1-b357-42ee-83a8-336522ed6cbf');
$requestRequestBody->setDisplayName('Users from connected organizations can request');
$requestRequestBody->setDescription('Allow users from configured connected organizations to request and be approved by their sponsors');
$requestRequestBody->setCanExtend(False);
$requestRequestBody->setDurationInDays(365);
$requestRequestBody->setExpirationDateTime(null);

$requestorSettings = new RequestorSettings();
$requestRequestBody->setRequestorSettings($requestorSettings);


$requestorSettings->setScopeType('AllExistingConnectedOrganizationSubjects');
$requestorSettings->setAcceptRequests(True);


$requestApprovalSettings = new ApprovalSettings();
$requestRequestBody->setRequestApprovalSettings($requestApprovalSettings);


$requestApprovalSettings->setIsApprovalRequired(True);
$requestApprovalSettings->setIsApprovalRequiredForExtension(False);
$requestApprovalSettings->setIsRequestorJustificationRequired(True);
$requestApprovalSettings->setApprovalMode('SingleStage');
$approvalStagesArray = [];

$approvalStagesapprovalStages1 = new ApprovalStage();

$approvalStagesapprovalStages1->setApprovalStageTimeOutInDays(14);
$approvalStagesapprovalStages1->setIsApproverJustificationRequired(True);
$approvalStagesapprovalStages1->setIsEscalationEnabled(False);
$approvalStagesapprovalStages1->setEscalationTimeInMinutes(11520);
$primaryApproversArray = [];

$primaryApproversprimaryApprovers1 = new UserSet();

$primaryApproversprimaryApprovers1->setIsBackup(True);
$primaryApproversprimaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"id" => 'd2dcb9a1-a445-42ee-83a8-476522ed6cbf',
"description" => 'group for users from connected organizations which have no external sponsor',
];
$primaryApproversprimaryApprovers1->setAdditionalData($primaryApproversprimaryApprovers1AdditionalData);

$primaryApproversArray []= $primaryApproversprimaryApprovers1;

$primaryApproversprimaryApprovers2 = new UserSet();

$primaryApproversprimaryApprovers2->setIsBackup(False);
$primaryApproversprimaryApprovers2AdditionalData = [
"@odata.type" => '#microsoft.graph.externalSponsors',
];
$primaryApproversprimaryApprovers2->setAdditionalData($primaryApproversprimaryApprovers2AdditionalData);

$primaryApproversArray []= $primaryApproversprimaryApprovers2;
$approvalStagesapprovalStages1->setPrimaryApprovers($primaryApproversArray);

$approvalStagesArray []= $approvalStagesapprovalStages1;
$requestApprovalSettings->setApprovalStages($approvalStagesArray);

$questionsArray = [];

$questionsquestions1 = new AccessPackageQuestion();

$questionsquestions1->setIsRequired(False);

$text = new AccessPackageLocalizedContent();
$questionsquestions1->setText($text);


$text->setDefaultText('what state are you from?');
$localizedTextsArray = [];

$localizedTextslocalizedTexts1 = new AccessPackageLocalizedText();

$localizedTextslocalizedTexts1->setText('¿De qué estado eres?');
$localizedTextslocalizedTexts1->setLanguageCode('es');

$localizedTextsArray []= $localizedTextslocalizedTexts1;
$text->setLocalizedTexts($localizedTextsArray);

$questionsquestions1AdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageMultipleChoiceQuestion',
"choices" => [],
"allowsMultipleSelection" => False,
];
$questionsquestions1->setAdditionalData($questionsquestions1AdditionalData);

$questionsArray []= $questionsquestions1;

$questionsquestions2 = new AccessPackageQuestion();

$questionsquestions2->setIsRequired(False);

$text = new AccessPackageLocalizedContent();
$questionsquestions2->setText($text);


$text->setDefaultText('Who is your manager?');
$localizedTextsArray = [];

$localizedTextslocalizedTexts1 = new AccessPackageLocalizedText();

$localizedTextslocalizedTexts1->setText('por qué necesita acceso a este paquete');
$localizedTextslocalizedTexts1->setLanguageCode('es');

$localizedTextsArray []= $localizedTextslocalizedTexts1;
$text->setLocalizedTexts($localizedTextsArray);

$questionsquestions2AdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageTextInputQuestion',
"isSingleLineQuestion" => False,
];
$questionsquestions2->setAdditionalData($questionsquestions2AdditionalData);

$questionsArray []= $questionsquestions2;
$requestRequestBody->setQuestions($questionsArray);
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentPolicies()->post($requestRequestBody);


```