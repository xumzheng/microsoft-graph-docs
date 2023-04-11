---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleManagementPolicyRule()
request_body.@odatatype = '#microsoft.graph.unifiedRoleManagementPolicyEnablementRule'

request_body.id = 'Enablement_EndUser_Assignment'

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
'enabledRules' => ['Justification', 'MultiFactorAuthentication', 'Ticketing', ],
];
request_body.additionaldata(additionalData)




request_configuration = UnifiedRoleManagementPolicyRuleRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.roleManagementPolicies_by_id('unifiedRoleManagementPolicy-id').rules_by_id('unifiedRoleManagementPolicyRule-id').patch(request_body = request_body)


```