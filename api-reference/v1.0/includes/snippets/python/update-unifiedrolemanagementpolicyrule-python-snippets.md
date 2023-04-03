---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UnifiedRoleManagementPolicyRule();
requestBody.set@odatatype('#microsoft.graph.unifiedRoleManagementPolicyExpirationRule');

requestBody.setId('Expiration_EndUser_Assignment');

target = UnifiedRoleManagementPolicyRuleTarget();
target.set@odatatype('microsoft.graph.unifiedRoleManagementPolicyRuleTarget');

target.setCaller('EndUser');

target.setOperations([target.setUnifiedRoleManagementPolicyRuleTargetOperations(UnifiedRoleManagementPolicyRuleTargetOperations('all'));
]);

target.setLevel('Assignment');

target.setInheritableSettings([]);

target.setEnforcedSettings([]);


requestBody.setTarget($target);
additionalData = [
'isExpirationRequired' => true,
'maximumDuration' => 'PT1H45M', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.policies().roleManagementPoliciesById('unifiedRoleManagementPolicy-id').rulesById('unifiedRoleManagementPolicyRule-id').patch(requestBody);


```