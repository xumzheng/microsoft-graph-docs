---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.setDisplayName('Sales department users')

request_body.setDescription('All users from sales department')

request_body.setAllowedTargetScope(AllowedTargetScope('specificdirectoryusers'))

specificAllowedTargetsSubjectSet1 = SubjectSet()
specificAllowedTargetsSubjectSet1.set@odatatype('#microsoft.graph.attributeRuleMembers')

additionalData = [
'description' => 'Membership rule for all users from sales department', 
'membershipRule' => '(user.department -eq \"Sales\")', 
];
specificAllowedTargetsSubjectSet1.setAdditionalData(additionalData)



specificAllowedTargetsArray []= specificAllowedTargetsSubjectSet1;
request_body.setSpecificAllowedTargets(specificAllowedTargetsArray)


automaticRequestSettings = AccessPackageAutomaticRequestSettings()
automaticRequestSettings.setRequestAccessForAllowedTargets(true)


request_body.setAutomaticRequestSettings($automaticRequestSettings)
accessPackage = AccessPackage()
accessPackage.setId('8a36831e-1527-4b2b-aff2-81259a8d8e76')


request_body.setAccessPackage($accessPackage)


result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body, headers=)


```