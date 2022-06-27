---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageAssignmentPolicy();


$requestRequestBody->setDisplayName('policy for external access requests');
$requestRequestBody->setDescription('policy for users from connected organizations to request access, with two stages of approval.');
$requestRequestBody->setAllowedTargetScope(new AllowedTargetScope('allConfiguredConnectedOrganizationUsers'));
$specificAllowedTargetsArray = [];
$requestRequestBody->setSpecificAllowedTargets($specificAllowedTargetsArray);

$expiration = new ExpirationPattern();
$requestRequestBody->setExpiration($expiration);


$expiration->setType(new ExpirationPatternType('noExpiration'));


$requestorSettings = new AccessPackageAssignmentRequestorSettings();
$requestRequestBody->setRequestorSettings($requestorSettings);


$requestorSettings->setEnableTargetsToSelfAddAccess(True);
$requestorSettings->setEnableTargetsToSelfUpdateAccess(True);
$requestorSettings->setEnableTargetsToSelfRemoveAccess(True);
$requestorSettings->setAllowCustomAssignmentSchedule(False);
$requestorSettings->setEnableOnBehalfRequestorsToAddAccess(False);
$requestorSettings->setEnableOnBehalfRequestorsToUpdateAccess(False);
$requestorSettings->setEnableOnBehalfRequestorsToRemoveAccess(False);
$onBehalfRequestorsArray = [];
$requestorSettings->setOnBehalfRequestors($onBehalfRequestorsArray);


$requestApprovalSettings = new AccessPackageAssignmentApprovalSettings();
$requestRequestBody->setRequestApprovalSettings($requestApprovalSettings);


$requestApprovalSettings->setIsApprovalRequiredForAdd(True);
$requestApprovalSettings->setIsApprovalRequiredForUpdate(False);
$stagesArray = [];

$stagesstages1 = new AccessPackageApprovalStage();

$stagesstages1->setDurationBeforeAutomaticDenial('P14D');
$stagesstages1->setIsApproverJustificationRequired(False);
$stagesstages1->setIsEscalationEnabled(False);
$stagesstages1->setDurationBeforeEscalation('PT0S');
$primaryApproversArray = [];

$primaryApproversprimaryApprovers1 = new SubjectSet();

$primaryApproversprimaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.internalSponsors',
];
$primaryApproversprimaryApprovers1->setAdditionalData($primaryApproversprimaryApprovers1AdditionalData);

$primaryApproversArray []= $primaryApproversprimaryApprovers1;
$stagesstages1->setPrimaryApprovers($primaryApproversArray);
$fallbackPrimaryApproversArray = [];

$fallbackPrimaryApproversfallbackPrimaryApprovers1 = new SubjectSet();

$fallbackPrimaryApproversfallbackPrimaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.singleUser',
"userId" => '7deff43e-1f17-44ef-9e5f-d516b0ba11d4',
];
$fallbackPrimaryApproversfallbackPrimaryApprovers1->setAdditionalData($fallbackPrimaryApproversfallbackPrimaryApprovers1AdditionalData);

$fallbackPrimaryApproversArray []= $fallbackPrimaryApproversfallbackPrimaryApprovers1;

$fallbackPrimaryApproversfallbackPrimaryApprovers2 = new SubjectSet();

$fallbackPrimaryApproversfallbackPrimaryApprovers2AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"groupId" => '1623f912-5e86-41c2-af47-39dd67582b66',
];
$fallbackPrimaryApproversfallbackPrimaryApprovers2->setAdditionalData($fallbackPrimaryApproversfallbackPrimaryApprovers2AdditionalData);

$fallbackPrimaryApproversArray []= $fallbackPrimaryApproversfallbackPrimaryApprovers2;
$stagesstages1->setFallbackPrimaryApprovers($fallbackPrimaryApproversArray);
$escalationApproversArray = [];
$stagesstages1->setEscalationApprovers($escalationApproversArray);
$fallbackEscalationApproversArray = [];
$stagesstages1->setFallbackEscalationApprovers($fallbackEscalationApproversArray);

$stagesArray []= $stagesstages1;

$stagesstages2 = new AccessPackageApprovalStage();

$stagesstages2->setDurationBeforeAutomaticDenial('P14D');
$stagesstages2->setIsApproverJustificationRequired(False);
$stagesstages2->setIsEscalationEnabled(False);
$stagesstages2->setDurationBeforeEscalation('PT0S');
$primaryApproversArray = [];
$stagesstages2->setPrimaryApprovers($primaryApproversArray);
$fallbackPrimaryApproversArray = [];

$fallbackPrimaryApproversfallbackPrimaryApprovers1 = new SubjectSet();

$fallbackPrimaryApproversfallbackPrimaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.singleUser',
"userId" => '46184453-e63b-4f20-86c2-c557ed5d5df9',
];
$fallbackPrimaryApproversfallbackPrimaryApprovers1->setAdditionalData($fallbackPrimaryApproversfallbackPrimaryApprovers1AdditionalData);

$fallbackPrimaryApproversArray []= $fallbackPrimaryApproversfallbackPrimaryApprovers1;

$fallbackPrimaryApproversfallbackPrimaryApprovers2 = new SubjectSet();

$fallbackPrimaryApproversfallbackPrimaryApprovers2AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"groupId" => '1623f912-5e86-41c2-af47-39dd67582b66',
];
$fallbackPrimaryApproversfallbackPrimaryApprovers2->setAdditionalData($fallbackPrimaryApproversfallbackPrimaryApprovers2AdditionalData);

$fallbackPrimaryApproversArray []= $fallbackPrimaryApproversfallbackPrimaryApprovers2;
$stagesstages2->setFallbackPrimaryApprovers($fallbackPrimaryApproversArray);
$escalationApproversArray = [];
$stagesstages2->setEscalationApprovers($escalationApproversArray);
$fallbackEscalationApproversArray = [];
$stagesstages2->setFallbackEscalationApprovers($fallbackEscalationApproversArray);

$stagesArray []= $stagesstages2;
$requestApprovalSettings->setStages($stagesArray);


$reviewSettings = new AccessPackageAssignmentReviewSettings();
$requestRequestBody->setReviewSettings($reviewSettings);


$reviewSettings->setIsEnabled(True);
$reviewSettings->setExpirationBehavior(new AccessReviewExpirationBehavior('keepAccess'));
$reviewSettings->setIsRecommendationEnabled(True);
$reviewSettings->setIsReviewerJustificationRequired(True);
$reviewSettings->setIsSelfReview(False);

$schedule = new EntitlementManagementSchedule();
$reviewSettings->setSchedule($schedule);


$schedule->setStartDateTime(new DateTime("2022-07-02T06:59:59.998Z"));

$expiration = new ExpirationPattern();
$schedule->setExpiration($expiration);


$expiration->setDuration('P14D');
$expiration->setType(new ExpirationPatternType('afterDuration'));


$recurrence = new PatternedRecurrence();
$schedule->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('absoluteMonthly'));
$pattern->setInterval(3);
$pattern->setMonth(0);
$pattern->setDayOfMonth(0);
$daysOfWeekArray = [];
$pattern->setDaysOfWeek($daysOfWeekArray);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('noEnd'));
$range->setNumberOfOccurrences(0);



$primaryReviewersArray = [];

$primaryReviewersprimaryReviewers1 = new SubjectSet();

$primaryReviewersprimaryReviewers1AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"groupId" => '1623f912-5e86-41c2-af47-39dd67582b66',
];
$primaryReviewersprimaryReviewers1->setAdditionalData($primaryReviewersprimaryReviewers1AdditionalData);

$primaryReviewersArray []= $primaryReviewersprimaryReviewers1;
$reviewSettings->setPrimaryReviewers($primaryReviewersArray);
$fallbackReviewersArray = [];
$reviewSettings->setFallbackReviewers($fallbackReviewersArray);


$accessPackage = new AccessPackage();
$requestRequestBody->setAccessPackage($accessPackage);


$accessPackage->setId('a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b');

$result =  $graphClient->identityGovernance()->entitlementManagement()->assignmentPolicies()->post($requestRequestBody);


```