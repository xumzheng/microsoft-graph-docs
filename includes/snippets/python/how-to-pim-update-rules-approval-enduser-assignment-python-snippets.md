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

request_body.isApprovalRequired = true

request_body.isApprovalRequiredForExtension = false

request_body.isRequestorJustificationRequired = true

request_body.approvalMode = 'SingleStage'

approvalStages1 = ()
approvalStages1.@odatatype = 'microsoft.graph.unifiedApprovalStage'

approvalStages1.approvalStageTimeOutInDays = 1

approvalStages1.isApproverJustificationRequired = true

approvalStages1.escalationTimeInMinutes = 0

primaryApprovers1 = ()
primaryApprovers1.@odatatype = '#microsoft.graph.singleUser'

primaryApprovers1.userId = '10a08e2e-3ea2-4ce0-80cb-d5fdd4b05ea6'


primaryApproversArray []= primaryApprovers1;
primaryApprovers2 = ()
primaryApprovers2.@odatatype = '#microsoft.graph.groupMembers'

primaryApprovers2.groupId = '14f2746d-7d6f-4ac6-acd8-8cac318b041b'


primaryApproversArray []= primaryApprovers2;
approvalStages1.primaryapprovers(primaryApproversArray)


approvalStages1.isEscalationEnabled = false

approvalStages1.EscalationApprovers([])


approvalStagesArray []= approvalStages1;
request_body.approvalstages(approvalStagesArray)



request_body.setting = setting

];
request_body.additionaldata(additionalData)




request_configuration = UnifiedRoleManagementPolicyRuleRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.roleManagementPolicies_by_id('unifiedRoleManagementPolicy-id').rules_by_id('unifiedRoleManagementPolicyRule-id').patch(request_body = request_body)


```