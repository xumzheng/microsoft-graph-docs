---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleManagementPolicyRule()
request_body.@odatatype = '#microsoft.graph.unifiedRoleManagementPolicyApprovalRule'

request_body.id = 'Approval_EndUser_Assignment'

target = UnifiedRoleManagementPolicyRuleTarget()
target.@odatatype = 'microsoft.graph.unifiedRoleManagementPolicyRuleTarget'

target.caller = 'EndUser'

target.Operations([target.UnifiedRoleManagementPolicyRuleTargetOperations(UnifiedRoleManagementPolicyRuleTargetOperations('all'))
])

target.level = 'Assignment'

target.InheritableSettings([])

target.EnforcedSettings([])


request_body.target = target
additionalData = [
'setting' => request_body = Setting()
request_body.@odatatype = 'microsoft.graph.approvalSettings'

request_body.is_approval_required = True

request_body.is_approval_required_for_extension = False

request_body.is_requestor_justification_required = True

request_body.approvalMode = 'SingleStage'

approval_stages1 = ()
approvalStages1.@odatatype = 'microsoft.graph.unifiedApprovalStage'

approvalStages1.approval_stage_time_out_in_days = 1

approvalStages1.is_approver_justification_required = True

approvalStages1.escalation_time_in_minutes = 0

primary_approvers1 = ()
primaryApprovers1.@odatatype = '#microsoft.graph.singleUser'

primaryApprovers1.userId = '10a08e2e-3ea2-4ce0-80cb-d5fdd4b05ea6'


primaryApproversArray []= primaryApprovers1;
primary_approvers2 = ()
primaryApprovers2.@odatatype = '#microsoft.graph.groupMembers'

primaryApprovers2.groupId = '14f2746d-7d6f-4ac6-acd8-8cac318b041b'


primaryApproversArray []= primaryApprovers2;
approvalStages1.primaryapprovers(primaryApproversArray)


approvalStages1.is_escalation_enabled = False

approvalStages1.EscalationApprovers([])


approvalStagesArray []= approvalStages1;
request_body.approvalstages(approvalStagesArray)



request_body.setting = setting

];
request_body.additionaldata(additionalData)





result = await client.policies.roleManagementPolicies_by_id('unifiedRoleManagementPolicy-id').rules_by_id('unifiedRoleManagementPolicyRule-id').patch(request_body = request_body)


```