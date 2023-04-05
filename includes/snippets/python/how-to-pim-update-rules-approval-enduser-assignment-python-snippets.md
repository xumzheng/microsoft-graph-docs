---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleManagementPolicyRule()
request_body.set@odatatype('#microsoft.graph.unifiedRoleManagementPolicyApprovalRule')

request_body.setId('Approval_EndUser_Assignment')

target = UnifiedRoleManagementPolicyRuleTarget()
target.set@odatatype('microsoft.graph.unifiedRoleManagementPolicyRuleTarget')

target.setCaller('EndUser')

target.setOperations([target.setUnifiedRoleManagementPolicyRuleTargetOperations(UnifiedRoleManagementPolicyRuleTargetOperations('all'))
])

target.setLevel('Assignment')

target.setInheritableSettings([])

target.setEnforcedSettings([])


request_body.setTarget($target)
additionalData = [
'setting' => request_body = Setting()
request_body.set@odatatype('microsoft.graph.approvalSettings')

request_body.setIsApprovalRequired(true)

request_body.setIsApprovalRequiredForExtension(false)

request_body.setIsRequestorJustificationRequired(true)

request_body.setApprovalMode('SingleStage')

approvalStages1 = ()
approvalStages1.set@odatatype('microsoft.graph.unifiedApprovalStage')

approvalStages1.setApprovalStageTimeOutInDays(1)

approvalStages1.setIsApproverJustificationRequired(true)

approvalStages1.setEscalationTimeInMinutes(0)

primaryApprovers1 = ()
primaryApprovers1.set@odatatype('#microsoft.graph.singleUser')

primaryApprovers1.setUserId('10a08e2e-3ea2-4ce0-80cb-d5fdd4b05ea6')


primaryApproversArray []= primaryApprovers1;
primaryApprovers2 = ()
primaryApprovers2.set@odatatype('#microsoft.graph.groupMembers')

primaryApprovers2.setGroupId('14f2746d-7d6f-4ac6-acd8-8cac318b041b')


primaryApproversArray []= primaryApprovers2;
approvalStages1.setPrimaryApprovers(primaryApproversArray)


approvalStages1.setIsEscalationEnabled(false)

approvalStages1.setEscalationApprovers([])


approvalStagesArray []= approvalStages1;
request_body.setApprovalStages(approvalStagesArray)



request_body.setSetting($setting)

];
request_body.setAdditionalData(additionalData)




result = await client.policies.roleManagementPoliciesById('unifiedRoleManagementPolicy-id').rulesById('unifiedRoleManagementPolicyRule-id').patch(request_body)


```