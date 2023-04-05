---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleManagementPolicyRule()
request_body.set@odatatype('#microsoft.graph.unifiedRoleManagementPolicyExpirationRule')

request_body.setId('Expiration_EndUser_Assignment')

target = UnifiedRoleManagementPolicyRuleTarget()
target.set@odatatype('microsoft.graph.unifiedRoleManagementPolicyRuleTarget')

target.setCaller('EndUser')

target.setOperations(['All', ])

target.setLevel('Assignment')

target.setInheritableSettings([])

target.setEnforcedSettings([])


request_body.setTarget($target)
additionalData = [
'isExpirationRequired' => true,
'maximumDuration' => 'PT1H45M', 
];
request_body.setAdditionalData(additionalData)




result = await client.policies.roleManagementPoliciesby_id('unifiedRoleManagementPolicy-id').rulesby_id('unifiedRoleManagementPolicyRule-id').patch(request_body)


```