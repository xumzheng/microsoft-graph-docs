---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleManagementPolicyRule()
request_body.set@odatatype('#microsoft.graph.unifiedRoleManagementPolicyEnablementRule')

request_body.setId('Enablement_Admin_Assignment')

target = UnifiedRoleManagementPolicyRuleTarget()
target.set@odatatype('microsoft.graph.unifiedRoleManagementPolicyRuleTarget')

target.setCaller('Admin')

target.setOperations([target.setUnifiedRoleManagementPolicyRuleTargetOperations(UnifiedRoleManagementPolicyRuleTargetOperations('all'))
])

target.setLevel('Assignment')

target.setInheritableSettings([])

target.setEnforcedSettings([])


request_body.setTarget($target)
additionalData = [
'enabledRules' => ['Justification', 'MultiFactorAuthentication', ],
];
request_body.setAdditionalData(additionalData)




result = await client.policies.roleManagementPolicies_by_id('unifiedRoleManagementPolicy-id').rules_by_id('unifiedRoleManagementPolicyRule-id').patch(request_body)


```