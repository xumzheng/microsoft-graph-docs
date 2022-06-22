---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentPolicy();


$requestRequestBody->setAccessPackageId('string (identifier)');
$requestRequestBody->setDisplayName('Users from connected organizations can request');
$requestRequestBody->setDescription('Allow users from configured connected organizations to request and be approved by their sponsors');
$requestRequestBody->setCanExtend(False);
$requestRequestBody->setDurationInDays(365);
$requestRequestBody->setExpirationDateTime(null);

$requestorSettings = new RequestorSettings();
$requestRequestBody->setRequestorSettings($requestorSettings);


$requestorSettings->setScopeType('AllExistingConnectedOrganizationSubjects');
$requestorSettings->setAcceptRequests(True);
$allowedRequestorsArray = [];
$requestorSettings->setAllowedRequestors($allowedRequestorsArray);


$requestApprovalSettings = new ApprovalSettings();
$requestRequestBody->setRequestApprovalSettings($requestApprovalSettings);


$requestApprovalSettings->setIsApprovalRequired(True);
$requestApprovalSettings->setIsApprovalRequiredForExtension(False);
$requestApprovalSettings->setIsRequestorJustificationRequired(True);
$requestApprovalSettings->setApprovalMode('Serial');
$approvalStagesArray = [];

$approvalStages1 = new ApprovalStage();

$approvalStages1->setApprovalStageTimeOutInDays(14);
$approvalStages1->setIsApproverJustificationRequired(True);
$approvalStages1->setIsEscalationEnabled(True);
$approvalStages1->setEscalationTimeInMinutes(11520);
$primaryApproversArray = [];

$primaryApprovers1 = new UserSet();

$primaryApprovers1->setIsBackup(True);
$primaryApprovers1AdditionalData = [
		"@odata.type" => '#microsoft.graph.groupMembers',
		"id" => 'string (identifier)',
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
$escalationApproversArray = [];

$escalationApprovers1 = new UserSet();

$escalationApprovers1->setIsBackup(True);
$escalationApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.singleUser',
"id" => 'string (identifier)',
"description" => 'user if the external sponsor does not respond',
];
$escalationApprovers1->setAdditionalData($escalationApprovers1AdditionalData);

$escalationApproversArray []= $escalationApprovers1;
$approvalStages1->setEscalationApprovers($escalationApproversArray);

$approvalStagesArray []= $approvalStages1;

$approvalStages2 = new ApprovalStage();

$approvalStages2->setApprovalStageTimeOutInDays(14);
$approvalStages2->setIsApproverJustificationRequired(True);
$approvalStages2->setIsEscalationEnabled(True);
$approvalStages2->setEscalationTimeInMinutes(11520);
$primaryApproversArray = [];

$primaryApprovers1 = new UserSet();

$primaryApprovers1->setIsBackup(True);
$primaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"id" => 'string (identifier)',
"description" => 'group for users from connected organizations which have no internal sponsor',
];
$primaryApprovers1->setAdditionalData($primaryApprovers1AdditionalData);

$primaryApproversArray []= $primaryApprovers1;

$primaryApprovers2 = new UserSet();

$primaryApprovers2->setIsBackup(False);
$primaryApprovers2AdditionalData = [
"@odata.type" => '#microsoft.graph.internalSponsors',
];
$primaryApprovers2->setAdditionalData($primaryApprovers2AdditionalData);

$primaryApproversArray []= $primaryApprovers2;
$approvalStages2->setPrimaryApprovers($primaryApproversArray);
$escalationApproversArray = [];

$escalationApprovers1 = new UserSet();

$escalationApprovers1->setIsBackup(True);
$escalationApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.singleUser',
"id" => 'string (identifier)',
"description" => 'user if the internal sponsor does not respond',
];
$escalationApprovers1->setAdditionalData($escalationApprovers1AdditionalData);

$escalationApproversArray []= $escalationApprovers1;
$approvalStages2->setEscalationApprovers($escalationApproversArray);

$approvalStagesArray []= $approvalStages2;
$requestApprovalSettings->setApprovalStages($approvalStagesArray);


$accessReviewSettings = new AssignmentReviewSettings();
$requestRequestBody->setAccessReviewSettings($accessReviewSettings);


$accessReviewSettings->setIsEnabled(True);
$accessReviewSettings->setRecurrenceType('quarterly');
$accessReviewSettings->setReviewerType('Self');
$accessReviewSettings->setStartDateTime(new DateTime("2020-04-01T07:59:59.998Z"));
$accessReviewSettings->setDurationInDays(25);
$reviewersArray = [];
$accessReviewSettings->setReviewers($reviewersArray);

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentPolicies()->post($requestRequestBody);


```