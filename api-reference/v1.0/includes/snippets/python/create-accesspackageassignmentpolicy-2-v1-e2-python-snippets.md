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
requestor_settings = AccessPackageAssignmentRequestorSettings()
requestorSettings.enable_targets_to_self_add_access = True

requestorSettings.enable_targets_to_self_update_access = True

requestorSettings.enable_targets_to_self_remove_access = True

requestorSettings.allow_custom_assignment_schedule = False

requestorSettings.enable_on_behalf_requestors_to_add_access = False

requestorSettings.enable_on_behalf_requestors_to_update_access = False

requestorSettings.enable_on_behalf_requestors_to_remove_access = False

requestorSettings.OnBehalfRequestors([])


request_body.requestor_settings = requestorSettings
request_approval_settings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.is_approval_required_for_add = True

requestApprovalSettings.is_approval_required_for_update = False

stages_access_package_approval_stage1 = AccessPackageApprovalStage()
stagesAccessPackageApprovalStage1.durationbeforeautomaticdenial =  \DateInterval('P14D')

stagesAccessPackageApprovalStage1.is_approver_justification_required = False

stagesAccessPackageApprovalStage1.is_escalation_enabled = False

stagesAccessPackageApprovalStage1.durationbeforeescalation =  \DateInterval('PT0S')

primary_approvers_subject_set1 = SubjectSet()
primaryApproversSubjectSet1.@odatatype = '#microsoft.graph.internalSponsors'


primaryApproversArray []= primaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.primaryapprovers(primaryApproversArray)


fallback_primary_approvers_subject_set1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.@odatatype = '#microsoft.graph.singleUser'

additionalData = [
'userId' => '7deff43e-1f17-44ef-9e5f-d516b0ba11d4', 
];
fallbackPrimaryApproversSubjectSet1.additionaldata(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
fallback_primary_approvers_subject_set2 = SubjectSet()
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
stages_access_package_approval_stage2 = AccessPackageApprovalStage()
stagesAccessPackageApprovalStage2.durationbeforeautomaticdenial =  \DateInterval('P14D')

stagesAccessPackageApprovalStage2.is_approver_justification_required = False

stagesAccessPackageApprovalStage2.is_escalation_enabled = False

stagesAccessPackageApprovalStage2.durationbeforeescalation =  \DateInterval('PT0S')

stagesAccessPackageApprovalStage2.PrimaryApprovers([])

fallback_primary_approvers_subject_set1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.@odatatype = '#microsoft.graph.singleUser'

additionalData = [
'userId' => '46184453-e63b-4f20-86c2-c557ed5d5df9', 
];
fallbackPrimaryApproversSubjectSet1.additionaldata(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
fallback_primary_approvers_subject_set2 = SubjectSet()
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



request_body.request_approval_settings = requestApprovalSettings
review_settings = AccessPackageAssignmentReviewSettings()
reviewSettings.is_enabled = True

reviewSettings.ExpirationBehavior(AccessReviewExpirationBehavior('keepaccess'))

reviewSettings.is_recommendation_enabled = True

reviewSettings.is_reviewer_justification_required = True

reviewSettings.is_self_review = False

review_settings_schedule = EntitlementManagementSchedule()
reviewSettingsSchedule.startDateTime = DateTime('2022-07-02T06:59:59.998Z')

review_settings_schedule_expiration = ExpirationPattern()
reviewSettingsScheduleExpiration.duration =  \DateInterval('P14D')

reviewSettingsScheduleExpiration.Type(ExpirationPatternType('afterduration'))


reviewSettingsSchedule.expiration = reviewSettingsScheduleExpiration
review_settings_schedule_recurrence = PatternedRecurrence()
review_settings_schedule_recurrence_pattern = RecurrencePattern()
reviewSettingsScheduleRecurrencePattern.Type(RecurrencePatternType('absolutemonthly'))

reviewSettingsScheduleRecurrencePattern.interval = 3

reviewSettingsScheduleRecurrencePattern.month = 0

reviewSettingsScheduleRecurrencePattern.day_of_month = 0

reviewSettingsScheduleRecurrencePattern.DaysOfWeek([])


reviewSettingsScheduleRecurrence.pattern = reviewSettingsScheduleRecurrencePattern
review_settings_schedule_recurrence_range = RecurrenceRange()
reviewSettingsScheduleRecurrenceRange.Type(RecurrenceRangeType('noend'))

reviewSettingsScheduleRecurrenceRange.number_of_occurrences = 0


reviewSettingsScheduleRecurrence.range = reviewSettingsScheduleRecurrenceRange

reviewSettingsSchedule.recurrence = reviewSettingsScheduleRecurrence

reviewSettings.schedule = reviewSettingsSchedule
primary_reviewers_subject_set1 = SubjectSet()
primaryReviewersSubjectSet1.@odatatype = '#microsoft.graph.groupMembers'

additionalData = [
'groupId' => '1623f912-5e86-41c2-af47-39dd67582b66', 
];
primaryReviewersSubjectSet1.additionaldata(additionalData)



primaryReviewersArray []= primaryReviewersSubjectSet1;
reviewSettings.primaryreviewers(primaryReviewersArray)


reviewSettings.FallbackReviewers([])


request_body.review_settings = reviewSettings
access_package = AccessPackage()
accessPackage.id = 'a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b'


request_body.access_package = accessPackage



result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body = request_body)


```