---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.displayName = 'policy for external access requests'

request_body.description = 'policy for users from connected organizations to request access, with two stages of approval.'

request_body.AllowedTargetScope(AllowedTargetScope('allconfiguredconnectedorganizationusers'))

request_body.SpecificAllowedTargets([])

expiration = ExpirationPattern()
expiration.Type(ExpirationPatternType('noexpiration'))


request_body.expiration = expiration
requestorSettings = AccessPackageAssignmentRequestorSettings()
requestorSettings.enableTargetsToSelfAddAccess = true

requestorSettings.enableTargetsToSelfUpdateAccess = true

requestorSettings.enableTargetsToSelfRemoveAccess = true

requestorSettings.allowCustomAssignmentSchedule = false

requestorSettings.enableOnBehalfRequestorsToAddAccess = false

requestorSettings.enableOnBehalfRequestorsToUpdateAccess = false

requestorSettings.enableOnBehalfRequestorsToRemoveAccess = false

requestorSettings.OnBehalfRequestors([])


request_body.requestorSettings = requestorSettings
requestApprovalSettings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.isApprovalRequiredForAdd = true

requestApprovalSettings.isApprovalRequiredForUpdate = false

stagesAccessPackageApprovalStage1 = AccessPackageApprovalStage()
stagesAccessPackageApprovalStage1.durationbeforeautomaticdenial =  \DateInterval('P14D')

stagesAccessPackageApprovalStage1.isApproverJustificationRequired = false

stagesAccessPackageApprovalStage1.isEscalationEnabled = false

stagesAccessPackageApprovalStage1.durationbeforeescalation =  \DateInterval('PT0S')

primaryApproversSubjectSet1 = SubjectSet()
primaryApproversSubjectSet1.@odatatype = '#microsoft.graph.internalSponsors'


primaryApproversArray []= primaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.primaryapprovers(primaryApproversArray)


fallbackPrimaryApproversSubjectSet1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.@odatatype = '#microsoft.graph.singleUser'

additionalData = [
'userId' => '7deff43e-1f17-44ef-9e5f-d516b0ba11d4', 
];
fallbackPrimaryApproversSubjectSet1.additionaldata(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
fallbackPrimaryApproversSubjectSet2 = SubjectSet()
fallbackPrimaryApproversSubjectSet2.@odatatype = '#microsoft.graph.groupMembers'

additionalData = [
'groupId' => '1623f912-5e86-41c2-af47-39dd67582b66', 
];
fallbackPrimaryApproversSubjectSet2.additionaldata(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet2;
stagesAccessPackageApprovalStage1.fallbackprimaryapprovers(fallbackPrimaryApproversArray)


stagesAccessPackageApprovalStage1.EscalationApprovers([])

stagesAccessPackageApprovalStage1.FallbackEscalationApprovers([])


stagesArray []= stagesAccessPackageApprovalStage1;
stagesAccessPackageApprovalStage2 = AccessPackageApprovalStage()
stagesAccessPackageApprovalStage2.durationbeforeautomaticdenial =  \DateInterval('P14D')

stagesAccessPackageApprovalStage2.isApproverJustificationRequired = false

stagesAccessPackageApprovalStage2.isEscalationEnabled = false

stagesAccessPackageApprovalStage2.durationbeforeescalation =  \DateInterval('PT0S')

stagesAccessPackageApprovalStage2.PrimaryApprovers([])

fallbackPrimaryApproversSubjectSet1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.@odatatype = '#microsoft.graph.singleUser'

additionalData = [
'userId' => '46184453-e63b-4f20-86c2-c557ed5d5df9', 
];
fallbackPrimaryApproversSubjectSet1.additionaldata(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
fallbackPrimaryApproversSubjectSet2 = SubjectSet()
fallbackPrimaryApproversSubjectSet2.@odatatype = '#microsoft.graph.groupMembers'

additionalData = [
'groupId' => '1623f912-5e86-41c2-af47-39dd67582b66', 
];
fallbackPrimaryApproversSubjectSet2.additionaldata(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet2;
stagesAccessPackageApprovalStage2.fallbackprimaryapprovers(fallbackPrimaryApproversArray)


stagesAccessPackageApprovalStage2.EscalationApprovers([])

stagesAccessPackageApprovalStage2.FallbackEscalationApprovers([])


stagesArray []= stagesAccessPackageApprovalStage2;
requestApprovalSettings.stages(stagesArray)



request_body.requestApprovalSettings = requestApprovalSettings
reviewSettings = AccessPackageAssignmentReviewSettings()
reviewSettings.isEnabled = true

reviewSettings.ExpirationBehavior(AccessReviewExpirationBehavior('keepaccess'))

reviewSettings.isRecommendationEnabled = true

reviewSettings.isReviewerJustificationRequired = true

reviewSettings.isSelfReview = false

reviewSettingsSchedule = EntitlementManagementSchedule()
reviewSettingsSchedule.startDateTime = DateTime('2022-07-02T06:59:59.998Z')

reviewSettingsScheduleExpiration = ExpirationPattern()
reviewSettingsScheduleExpiration.duration =  \DateInterval('P14D')

reviewSettingsScheduleExpiration.Type(ExpirationPatternType('afterduration'))


reviewSettingsSchedule.expiration = reviewSettingsScheduleExpiration
reviewSettingsScheduleRecurrence = PatternedRecurrence()
reviewSettingsScheduleRecurrencePattern = RecurrencePattern()
reviewSettingsScheduleRecurrencePattern.Type(RecurrencePatternType('absolutemonthly'))

reviewSettingsScheduleRecurrencePattern.interval = 3

reviewSettingsScheduleRecurrencePattern.month = 0

reviewSettingsScheduleRecurrencePattern.dayOfMonth = 0

reviewSettingsScheduleRecurrencePattern.DaysOfWeek([])


reviewSettingsScheduleRecurrence.pattern = reviewSettingsScheduleRecurrencePattern
reviewSettingsScheduleRecurrenceRange = RecurrenceRange()
reviewSettingsScheduleRecurrenceRange.Type(RecurrenceRangeType('noend'))

reviewSettingsScheduleRecurrenceRange.numberOfOccurrences = 0


reviewSettingsScheduleRecurrence.range = reviewSettingsScheduleRecurrenceRange

reviewSettingsSchedule.recurrence = reviewSettingsScheduleRecurrence

reviewSettings.schedule = reviewSettingsSchedule
primaryReviewersSubjectSet1 = SubjectSet()
primaryReviewersSubjectSet1.@odatatype = '#microsoft.graph.groupMembers'

additionalData = [
'groupId' => '1623f912-5e86-41c2-af47-39dd67582b66', 
];
primaryReviewersSubjectSet1.additionaldata(additionalData)



primaryReviewersArray []= primaryReviewersSubjectSet1;
reviewSettings.primaryreviewers(primaryReviewersArray)


reviewSettings.FallbackReviewers([])


request_body.reviewSettings = reviewSettings
accessPackage = AccessPackage()
accessPackage.id = 'a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b'


request_body.accessPackage = accessPackage


request_configuration = AssignmentPoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body = request_body)


```