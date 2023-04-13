---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.id = '87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187'

request_body.displayName = 'All Users'

request_body.description = 'All users can request for access to the directory.'

request_body.AllowedTargetScope(AllowedTargetScope('alldirectoryusers'))

request_body.automaticRequestSettings=null

request_body.SpecificAllowedTargets([])

expiration = ExpirationPattern()
expiration.Type(ExpirationPatternType('noexpiration'))


request_body.expiration = expiration
requestor_settings = AccessPackageAssignmentRequestorSettings()
requestorSettings.enable_targets_to_self_add_access = True

requestorSettings.enable_targets_to_self_update_access = False

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
stagesAccessPackageApprovalStage1.durationbeforeautomaticdenial =  \DateInterval('P2D')

stagesAccessPackageApprovalStage1.is_approver_justification_required = False

stagesAccessPackageApprovalStage1.is_escalation_enabled = False

stagesAccessPackageApprovalStage1.durationbeforeescalation =  \DateInterval('PT0S')

primary_approvers_subject_set1 = SubjectSet()
primaryApproversSubjectSet1.@odatatype = '#microsoft.graph.requestorManager'

additionalData = [
'managerLevel' => 1,
];
primaryApproversSubjectSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.primaryapprovers(primaryApproversArray)


fallback_primary_approvers_subject_set1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.@odatatype = '#microsoft.graph.singleUser'

additionalData = [
'userId' => 'e6bf4d7d-6824-4dd0-809d-5bf42d4817c2', 
'description' => 'user', 
];
fallbackPrimaryApproversSubjectSet1.additionaldata(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.fallbackprimaryapprovers(fallbackPrimaryApproversArray)


stagesAccessPackageApprovalStage1.EscalationApprovers([])

stagesAccessPackageApprovalStage1.FallbackEscalationApprovers([])


stagesArray []= stagesAccessPackageApprovalStage1;
requestApprovalSettings.stages(stagesArray)



request_body.request_approval_settings = requestApprovalSettings
access_package = AccessPackage()
accessPackage.id = '49d2c59b-0a81-463d-a8ec-ddad3935d8a0'


request_body.access_package = accessPackage



result = await client.identityGovernance.entitlementManagement.assignmentPolicies_by_id('accessPackageAssignmentPolicy-id').put(request_body = request_body)


```