---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.accessPackageId = 'string (identifier)'

request_body.displayName = 'Users from connected organizations can request'

request_body.description = 'Allow users from configured connected organizations to request and be approved by their sponsors'

request_body.can_extend = False

request_body.duration_in_days = 365

request_body.expirationDateTime=null

requestor_settings = RequestorSettings()
requestorSettings.scopeType = 'AllExistingConnectedOrganizationSubjects'

requestorSettings.accept_requests = True

requestorSettings.AllowedRequestors([])


request_body.requestor_settings = requestorSettings
request_approval_settings = ApprovalSettings()
requestApprovalSettings.is_approval_required = True

requestApprovalSettings.is_approval_required_for_extension = False

requestApprovalSettings.is_requestor_justification_required = True

requestApprovalSettings.approvalMode = 'Serial'

approval_stages_approval_stage1 = ApprovalStage()
approvalStagesApprovalStage1.approval_stage_time_out_in_days = 14

approvalStagesApprovalStage1.is_approver_justification_required = True

approvalStagesApprovalStage1.is_escalation_enabled = True

approvalStagesApprovalStage1.escalation_time_in_minutes = 11520

primary_approvers_user_set1 = UserSet()
primaryApproversUserSet1.@odatatype = '#microsoft.graph.groupMembers'

primaryApproversUserSet1.is_backup = True

additionalData = [
'id' => 'string (identifier)', 
'description' => 'group for users from connected organizations which have no external sponsor', 
];
primaryApproversUserSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversUserSet1;
primary_approvers_user_set2 = UserSet()
primaryApproversUserSet2.@odatatype = '#microsoft.graph.externalSponsors'

primaryApproversUserSet2.is_backup = False


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage1.primaryapprovers(primaryApproversArray)


escalation_approvers_user_set1 = UserSet()
escalationApproversUserSet1.@odatatype = '#microsoft.graph.singleUser'

escalationApproversUserSet1.is_backup = True

additionalData = [
'id' => 'string (identifier)', 
'description' => 'user if the external sponsor does not respond', 
];
escalationApproversUserSet1.additionaldata(additionalData)



escalationApproversArray []= escalationApproversUserSet1;
approvalStagesApprovalStage1.escalationapprovers(escalationApproversArray)



approvalStagesArray []= approvalStagesApprovalStage1;
approval_stages_approval_stage2 = ApprovalStage()
approvalStagesApprovalStage2.approval_stage_time_out_in_days = 14

approvalStagesApprovalStage2.is_approver_justification_required = True

approvalStagesApprovalStage2.is_escalation_enabled = True

approvalStagesApprovalStage2.escalation_time_in_minutes = 11520

primary_approvers_user_set1 = UserSet()
primaryApproversUserSet1.@odatatype = '#microsoft.graph.groupMembers'

primaryApproversUserSet1.is_backup = True

additionalData = [
'id' => 'string (identifier)', 
'description' => 'group for users from connected organizations which have no internal sponsor', 
];
primaryApproversUserSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversUserSet1;
primary_approvers_user_set2 = UserSet()
primaryApproversUserSet2.@odatatype = '#microsoft.graph.internalSponsors'

primaryApproversUserSet2.is_backup = False


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage2.primaryapprovers(primaryApproversArray)


escalation_approvers_user_set1 = UserSet()
escalationApproversUserSet1.@odatatype = '#microsoft.graph.singleUser'

escalationApproversUserSet1.is_backup = True

additionalData = [
'id' => 'string (identifier)', 
'description' => 'user if the internal sponsor does not respond', 
];
escalationApproversUserSet1.additionaldata(additionalData)



escalationApproversArray []= escalationApproversUserSet1;
approvalStagesApprovalStage2.escalationapprovers(escalationApproversArray)



approvalStagesArray []= approvalStagesApprovalStage2;
requestApprovalSettings.approvalstages(approvalStagesArray)



request_body.request_approval_settings = requestApprovalSettings
access_review_settings = AssignmentReviewSettings()
accessReviewSettings.is_enabled = True

accessReviewSettings.recurrenceType = 'quarterly'

accessReviewSettings.reviewerType = 'Self'

accessReviewSettings.startDateTime = DateTime('2020-04-01T07:59:59.998Z')

accessReviewSettings.duration_in_days = 25

accessReviewSettings.Reviewers([])


request_body.access_review_settings = accessReviewSettings



result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```