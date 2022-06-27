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

$approvalStagesapprovalStages1 = new ApprovalStage();

$approvalStagesapprovalStages1->setApprovalStageTimeOutInDays(14);
$approvalStagesapprovalStages1->setIsApproverJustificationRequired(True);
$approvalStagesapprovalStages1->setIsEscalationEnabled(True);
$approvalStagesapprovalStages1->setEscalationTimeInMinutes(11520);
$primaryApproversArray = [];

$primaryApproversprimaryApprovers1 = new UserSet();

$primaryApproversprimaryApprovers1->setIsBackup(True);
$primaryApproversprimaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"id" => 'string (identifier)',
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
$escalationApproversArray = [];

$escalationApproversescalationApprovers1 = new UserSet();

$escalationApproversescalationApprovers1->setIsBackup(True);
$escalationApproversescalationApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.singleUser',
"id" => 'string (identifier)',
"description" => 'user if the external sponsor does not respond',
];
$escalationApproversescalationApprovers1->setAdditionalData($escalationApproversescalationApprovers1AdditionalData);

$escalationApproversArray []= $escalationApproversescalationApprovers1;
$approvalStagesapprovalStages1->setEscalationApprovers($escalationApproversArray);

$approvalStagesArray []= $approvalStagesapprovalStages1;

$approvalStagesapprovalStages2 = new ApprovalStage();

$approvalStagesapprovalStages2->setApprovalStageTimeOutInDays(14);
$approvalStagesapprovalStages2->setIsApproverJustificationRequired(True);
$approvalStagesapprovalStages2->setIsEscalationEnabled(True);
$approvalStagesapprovalStages2->setEscalationTimeInMinutes(11520);
$primaryApproversArray = [];

$primaryApproversprimaryApprovers1 = new UserSet();

$primaryApproversprimaryApprovers1->setIsBackup(True);
$primaryApproversprimaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"id" => 'string (identifier)',
"description" => 'group for users from connected organizations which have no internal sponsor',
];
$primaryApproversprimaryApprovers1->setAdditionalData($primaryApproversprimaryApprovers1AdditionalData);

$primaryApproversArray []= $primaryApproversprimaryApprovers1;

$primaryApproversprimaryApprovers2 = new UserSet();

$primaryApproversprimaryApprovers2->setIsBackup(False);
$primaryApproversprimaryApprovers2AdditionalData = [
"@odata.type" => '#microsoft.graph.internalSponsors',
];
$primaryApproversprimaryApprovers2->setAdditionalData($primaryApproversprimaryApprovers2AdditionalData);

$primaryApproversArray []= $primaryApproversprimaryApprovers2;
$approvalStagesapprovalStages2->setPrimaryApprovers($primaryApproversArray);
$escalationApproversArray = [];

$escalationApproversescalationApprovers1 = new UserSet();

$escalationApproversescalationApprovers1->setIsBackup(True);
$escalationApproversescalationApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.singleUser',
"id" => 'string (identifier)',
"description" => 'user if the internal sponsor does not respond',
];
$escalationApproversescalationApprovers1->setAdditionalData($escalationApproversescalationApprovers1AdditionalData);

$escalationApproversArray []= $escalationApproversescalationApprovers1;
$approvalStagesapprovalStages2->setEscalationApprovers($escalationApproversArray);

$approvalStagesArray []= $approvalStagesapprovalStages2;
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