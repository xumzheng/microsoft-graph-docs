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

$approvalStages1 = new ApprovalStage();

$approvalStages1->setApprovalStageTimeOutInDays(14);
$approvalStages1->setIsApproverJustificationRequired(True);
$approvalStages1->setIsEscalationEnabled(False);
$approvalStages1->setEscalationTimeInMinutes(11520);
$primaryApproversArray = [];

$primaryApprovers1 = new UserSet();

$primaryApprovers1->setIsBackup(True);
$primaryApprovers1AdditionalData = [
		"@odata.type" => '#microsoft.graph.groupMembers',
		"id" => 'd2dcb9a1-a445-42ee-83a8-476522ed6cbf',
		"description" => 'group for users from connected organizations which have no external sponsor',
	];
$primaryApprovers1->setAdditionalData($primaryApprovers1AdditionalData);

$primaryApproversArray []= $primaryApprovers1;

$primaryApprovers2 = new UserSet();

$primaryApprovers2->setIsBackup(False);
$primaryApprovers2AdditionalData = [
	"@odata.type" => '#microsoft.graph.externalSponsors',
];
$primaryApprovers2->setAdditionalData($primaryApprovers2AdditionalData);

$primaryApproversArray []= $primaryApprovers2;
$approvalStages1->setPrimaryApprovers($primaryApproversArray);

$approvalStagesArray []= $approvalStages1;
$requestApprovalSettings->setApprovalStages($approvalStagesArray);

$questionsArray = [];

$questions1 = new AccessPackageQuestion();

$questions1->setIsRequired(False);

$text = new AccessPackageLocalizedContent();
$questions1->setText($text);


$text->setDefaultText('what state are you from?');
$localizedTextsArray = [];

$localizedTexts1 = new AccessPackageLocalizedText();

$localizedTexts1->setText('¿De qué estado eres?');
$localizedTexts1->setLanguageCode('es');

$localizedTextsArray []= $localizedTexts1;
$text->setLocalizedTexts($localizedTextsArray);

$questions1AdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageMultipleChoiceQuestion',
"choices" =>  [
],
"allowsMultipleSelection" => False,
];
$questions1->setAdditionalData($questions1AdditionalData);

$questionsArray []= $questions1;

$questions2 = new AccessPackageQuestion();

$questions2->setIsRequired(False);

$text = new AccessPackageLocalizedContent();
$questions2->setText($text);


$text->setDefaultText('Who is your manager?');
$localizedTextsArray = [];

$localizedTexts1 = new AccessPackageLocalizedText();

$localizedTexts1->setText('por qué necesita acceso a este paquete');
$localizedTexts1->setLanguageCode('es');

$localizedTextsArray []= $localizedTexts1;
$text->setLocalizedTexts($localizedTextsArray);

$questions2AdditionalData = [
"@odata.type" => '#microsoft.graph.accessPackageTextInputQuestion',
"isSingleLineQuestion" => False,
];
$questions2->setAdditionalData($questions2AdditionalData);

$questionsArray []= $questions2;
$requestRequestBody->setQuestions($questionsArray);
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentPolicies()->post($requestRequestBody);


```