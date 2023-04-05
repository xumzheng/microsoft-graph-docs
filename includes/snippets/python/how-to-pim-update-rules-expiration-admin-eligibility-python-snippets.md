---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleManagementPolicyRule()
request_body.set@odatatype('#microsoft.graph.unifiedRoleManagementPolicyExpirationRule')

request_body.setId('Expiration_Admin_Eligibility')

target = UnifiedRoleManagementPolicyRuleTarget()
target.set@odatatype('microsoft.graph.unifiedRoleManagementPolicyRuleTarget')

target.setCaller('Admin')

target.setOperations([target.setUnifiedRoleManagementPolicyRuleTargetOperations(UnifiedRoleManagementPolicyRuleTargetOperations('all'))
])

target.setLevel('Eligibility')

target.setInheritableSettings([])

target.setEnforcedSettings([])


request_body.setTarget($target)
additionalData = [
'isExpirationRequired' => true,
'maximumDuration' => 'P90D', 
];
request_body.setAdditionalData(additionalData)




result = await client.policies_roleManagementPoliciesby_id('unifiedRoleManagementPolicy-id')_rulesby_id('unifiedRoleManagementPolicyRule-id').patch(request_body)


```