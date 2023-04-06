---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleManagementPolicyRule()
request_body.set@odatatype('#microsoft.graph.unifiedRoleManagementPolicyEnablementRule')

request_body.setId('Enablement_EndUser_Assignment')

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
'enabledRules' => ['Justification', 'MultiFactorAuthentication', 'Ticketing', ],
];
request_body.setAdditionalData(additionalData)



request_config = UnifiedRoleManagementPolicyRuleRequestBuilderPatchRequestConfiguration(
request_config = UnifiedRoleManagementPolicyRuleRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.policies.roleManagementPolicies_by_id('unifiedRoleManagementPolicy-id').rules_by_id('unifiedRoleManagementPolicyRule-id').patch(request_body, headers=)


```