---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleManagementPolicyRule()
request_body.@odatatype = '#microsoft.graph.unifiedRoleManagementPolicyExpirationRule'

request_body.id = 'Expiration_Admin_Eligibility'

target = UnifiedRoleManagementPolicyRuleTarget()
target.@odatatype = 'microsoft.graph.unifiedRoleManagementPolicyRuleTarget'

target.caller = 'Admin'

target.Operations([target.UnifiedRoleManagementPolicyRuleTargetOperations(UnifiedRoleManagementPolicyRuleTargetOperations('all'))
])

target.level = 'Eligibility'

target.InheritableSettings([])

target.EnforcedSettings([])


request_body.target = target
additionalData = [
'isExpirationRequired' => true,
'maximumDuration' => 'P90D', 
];
request_body.additionaldata(additionalData)





result = await client.policies.roleManagementPolicies_by_id('unifiedRoleManagementPolicy-id').rules_by_id('unifiedRoleManagementPolicyRule-id').patch(request_body = request_body)


```