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

$stages1 = new AccessPackageApprovalStage();

$stages1->setDurationBeforeAutomaticDenial('P14D');
$stages1->setIsApproverJustificationRequired(False);
$stages1->setIsEscalationEnabled(False);
$stages1->setDurationBeforeEscalation('PT0S');
$primaryApproversArray = [];

$primaryApprovers1 = new SubjectSet();

$primaryApprovers1AdditionalData = [
	"@odata.type" => '#microsoft.graph.internalSponsors',
];
$primaryApprovers1->setAdditionalData($primaryApprovers1AdditionalData);

$primaryApproversArray []= $primaryApprovers1;
$stages1->setPrimaryApprovers($primaryApproversArray);
$fallbackPrimaryApproversArray = [];

$fallbackPrimaryApprovers1 = new SubjectSet();

$fallbackPrimaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.singleUser',
"userId" => '7deff43e-1f17-44ef-9e5f-d516b0ba11d4',
];
$fallbackPrimaryApprovers1->setAdditionalData($fallbackPrimaryApprovers1AdditionalData);

$fallbackPrimaryApproversArray []= $fallbackPrimaryApprovers1;

$fallbackPrimaryApprovers2 = new SubjectSet();

$fallbackPrimaryApprovers2AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"groupId" => '1623f912-5e86-41c2-af47-39dd67582b66',
];
$fallbackPrimaryApprovers2->setAdditionalData($fallbackPrimaryApprovers2AdditionalData);

$fallbackPrimaryApproversArray []= $fallbackPrimaryApprovers2;
$stages1->setFallbackPrimaryApprovers($fallbackPrimaryApproversArray);
$escalationApproversArray = [];
$stages1->setEscalationApprovers($escalationApproversArray);
$fallbackEscalationApproversArray = [];
$stages1->setFallbackEscalationApprovers($fallbackEscalationApproversArray);

$stagesArray []= $stages1;

$stages2 = new AccessPackageApprovalStage();

$stages2->setDurationBeforeAutomaticDenial('P14D');
$stages2->setIsApproverJustificationRequired(False);
$stages2->setIsEscalationEnabled(False);
$stages2->setDurationBeforeEscalation('PT0S');
$primaryApproversArray = [];
$stages2->setPrimaryApprovers($primaryApproversArray);
$fallbackPrimaryApproversArray = [];

$fallbackPrimaryApprovers1 = new SubjectSet();

$fallbackPrimaryApprovers1AdditionalData = [
"@odata.type" => '#microsoft.graph.singleUser',
"userId" => '46184453-e63b-4f20-86c2-c557ed5d5df9',
];
$fallbackPrimaryApprovers1->setAdditionalData($fallbackPrimaryApprovers1AdditionalData);

$fallbackPrimaryApproversArray []= $fallbackPrimaryApprovers1;

$fallbackPrimaryApprovers2 = new SubjectSet();

$fallbackPrimaryApprovers2AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"groupId" => '1623f912-5e86-41c2-af47-39dd67582b66',
];
$fallbackPrimaryApprovers2->setAdditionalData($fallbackPrimaryApprovers2AdditionalData);

$fallbackPrimaryApproversArray []= $fallbackPrimaryApprovers2;
$stages2->setFallbackPrimaryApprovers($fallbackPrimaryApproversArray);
$escalationApproversArray = [];
$stages2->setEscalationApprovers($escalationApproversArray);
$fallbackEscalationApproversArray = [];
$stages2->setFallbackEscalationApprovers($fallbackEscalationApproversArray);

$stagesArray []= $stages2;
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

$primaryReviewers1 = new SubjectSet();

$primaryReviewers1AdditionalData = [
"@odata.type" => '#microsoft.graph.groupMembers',
"groupId" => '1623f912-5e86-41c2-af47-39dd67582b66',
];
$primaryReviewers1->setAdditionalData($primaryReviewers1AdditionalData);

$primaryReviewersArray []= $primaryReviewers1;
$reviewSettings->setPrimaryReviewers($primaryReviewersArray);
$fallbackReviewersArray = [];
$reviewSettings->setFallbackReviewers($fallbackReviewersArray);


$accessPackage = new AccessPackage();
$requestRequestBody->setAccessPackage($accessPackage);


$accessPackage->setId('a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b');

$result =  $graphClient->identityGovernance()->entitlementManagement()->assignmentPolicies()->post($requestRequestBody);


```