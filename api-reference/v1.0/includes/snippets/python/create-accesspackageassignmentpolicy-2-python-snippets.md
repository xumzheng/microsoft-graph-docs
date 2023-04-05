---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.setDisplayName('policy for external access requests')

request_body.setDescription('policy for users from connected organizations to request access, with two stages of approval.')

request_body.setAllowedTargetScope(AllowedTargetScope('allconfiguredconnectedorganizationusers'))

request_body.setSpecificAllowedTargets([])

expiration = ExpirationPattern()
expiration.setType(ExpirationPatternType('noexpiration'))


request_body.setExpiration($expiration)
requestorSettings = AccessPackageAssignmentRequestorSettings()
requestorSettings.setEnableTargetsToSelfAddAccess(true)

requestorSettings.setEnableTargetsToSelfUpdateAccess(true)

requestorSettings.setEnableTargetsToSelfRemoveAccess(true)

requestorSettings.setAllowCustomAssignmentSchedule(false)

requestorSettings.setEnableOnBehalfRequestorsToAddAccess(false)

requestorSettings.setEnableOnBehalfRequestorsToUpdateAccess(false)

requestorSettings.setEnableOnBehalfRequestorsToRemoveAccess(false)

requestorSettings.setOnBehalfRequestors([])


request_body.setRequestorSettings($requestorSettings)
requestApprovalSettings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.setIsApprovalRequiredForAdd(true)

requestApprovalSettings.setIsApprovalRequiredForUpdate(false)

stagesAccessPackageApprovalStage1 = AccessPackageApprovalStage()
$stagesAccessPackageApprovalStage1.setDurationBeforeAutomaticDenial( \DateInterval('P14D'))

stagesAccessPackageApprovalStage1.setIsApproverJustificationRequired(false)

stagesAccessPackageApprovalStage1.setIsEscalationEnabled(false)

$stagesAccessPackageApprovalStage1.setDurationBeforeEscalation( \DateInterval('PT0S'))

primaryApproversSubjectSet1 = SubjectSet()
primaryApproversSubjectSet1.set@odatatype('#microsoft.graph.internalSponsors')


primaryApproversArray []= primaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.setPrimaryApprovers(primaryApproversArray)


fallbackPrimaryApproversSubjectSet1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.set@odatatype('#microsoft.graph.singleUser')

additionalData = [
'userId' => '7deff43e-1f17-44ef-9e5f-d516b0ba11d4', 
];
fallbackPrimaryApproversSubjectSet1.setAdditionalData(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
fallbackPrimaryApproversSubjectSet2 = SubjectSet()
fallbackPrimaryApproversSubjectSet2.set@odatatype('#microsoft.graph.groupMembers')

additionalData = [
'groupId' => '1623f912-5e86-41c2-af47-39dd67582b66', 
];
fallbackPrimaryApproversSubjectSet2.setAdditionalData(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet2;
stagesAccessPackageApprovalStage1.setFallbackPrimaryApprovers(fallbackPrimaryApproversArray)


stagesAccessPackageApprovalStage1.setEscalationApprovers([])

stagesAccessPackageApprovalStage1.setFallbackEscalationApprovers([])


stagesArray []= stagesAccessPackageApprovalStage1;
stagesAccessPackageApprovalStage2 = AccessPackageApprovalStage()
$stagesAccessPackageApprovalStage2.setDurationBeforeAutomaticDenial( \DateInterval('P14D'))

stagesAccessPackageApprovalStage2.setIsApproverJustificationRequired(false)

stagesAccessPackageApprovalStage2.setIsEscalationEnabled(false)

$stagesAccessPackageApprovalStage2.setDurationBeforeEscalation( \DateInterval('PT0S'))

stagesAccessPackageApprovalStage2.setPrimaryApprovers([])

fallbackPrimaryApproversSubjectSet1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.set@odatatype('#microsoft.graph.singleUser')

additionalData = [
'userId' => '46184453-e63b-4f20-86c2-c557ed5d5df9', 
];
fallbackPrimaryApproversSubjectSet1.setAdditionalData(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
fallbackPrimaryApproversSubjectSet2 = SubjectSet()
fallbackPrimaryApproversSubjectSet2.set@odatatype('#microsoft.graph.groupMembers')

additionalData = [
'groupId' => '1623f912-5e86-41c2-af47-39dd67582b66', 
];
fallbackPrimaryApproversSubjectSet2.setAdditionalData(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet2;
stagesAccessPackageApprovalStage2.setFallbackPrimaryApprovers(fallbackPrimaryApproversArray)


stagesAccessPackageApprovalStage2.setEscalationApprovers([])

stagesAccessPackageApprovalStage2.setFallbackEscalationApprovers([])


stagesArray []= stagesAccessPackageApprovalStage2;
requestApprovalSettings.setStages(stagesArray)



request_body.setRequestApprovalSettings($requestApprovalSettings)
reviewSettings = AccessPackageAssignmentReviewSettings()
reviewSettings.setIsEnabled(true)

reviewSettings.setExpirationBehavior(AccessReviewExpirationBehavior('keepaccess'))

reviewSettings.setIsRecommendationEnabled(true)

reviewSettings.setIsReviewerJustificationRequired(true)

reviewSettings.setIsSelfReview(false)

reviewSettingsSchedule = EntitlementManagementSchedule()
reviewSettingsSchedule.setStartDateTime(DateTime('2022-07-02T06:59:59.998Z'))

reviewSettingsScheduleExpiration = ExpirationPattern()
$reviewSettingsScheduleExpiration.setDuration( \DateInterval('P14D'))

reviewSettingsScheduleExpiration.setType(ExpirationPatternType('afterduration'))


reviewSettingsSchedule.setExpiration($reviewSettingsScheduleExpiration)
reviewSettingsScheduleRecurrence = PatternedRecurrence()
reviewSettingsScheduleRecurrencePattern = RecurrencePattern()
reviewSettingsScheduleRecurrencePattern.setType(RecurrencePatternType('absolutemonthly'))

reviewSettingsScheduleRecurrencePattern.setInterval(3)

reviewSettingsScheduleRecurrencePattern.setMonth(0)

reviewSettingsScheduleRecurrencePattern.setDayOfMonth(0)

reviewSettingsScheduleRecurrencePattern.setDaysOfWeek([])


reviewSettingsScheduleRecurrence.setPattern($reviewSettingsScheduleRecurrencePattern)
reviewSettingsScheduleRecurrenceRange = RecurrenceRange()
reviewSettingsScheduleRecurrenceRange.setType(RecurrenceRangeType('noend'))

reviewSettingsScheduleRecurrenceRange.setNumberOfOccurrences(0)


reviewSettingsScheduleRecurrence.setRange($reviewSettingsScheduleRecurrenceRange)

reviewSettingsSchedule.setRecurrence($reviewSettingsScheduleRecurrence)

reviewSettings.setSchedule($reviewSettingsSchedule)
primaryReviewersSubjectSet1 = SubjectSet()
primaryReviewersSubjectSet1.set@odatatype('#microsoft.graph.groupMembers')

additionalData = [
'groupId' => '1623f912-5e86-41c2-af47-39dd67582b66', 
];
primaryReviewersSubjectSet1.setAdditionalData(additionalData)



primaryReviewersArray []= primaryReviewersSubjectSet1;
reviewSettings.setPrimaryReviewers(primaryReviewersArray)


reviewSettings.setFallbackReviewers([])


request_body.setReviewSettings($reviewSettings)
accessPackage = AccessPackage()
accessPackage.setId('a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b')


request_body.setAccessPackage($accessPackage)


result = await client.identityGovernance_entitlementManagement_assignmentPolicies.post(request_body)


```