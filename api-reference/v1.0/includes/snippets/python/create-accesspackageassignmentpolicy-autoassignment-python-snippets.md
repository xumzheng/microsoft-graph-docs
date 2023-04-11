---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.displayName = 'Sales department users'

request_body.description = 'All users from sales department'

request_body.AllowedTargetScope(AllowedTargetScope('specificdirectoryusers'))

specificAllowedTargetsSubjectSet1 = SubjectSet()
specificAllowedTargetsSubjectSet1.@odatatype = '#microsoft.graph.attributeRuleMembers'

additionalData = [
'description' => 'Membership rule for all users from sales department', 
'membershipRule' => '(user.department -eq \"Sales\")', 
];
specificAllowedTargetsSubjectSet1.additionaldata(additionalData)



specificAllowedTargetsArray []= specificAllowedTargetsSubjectSet1;
request_body.specificallowedtargets(specificAllowedTargetsArray)


automaticRequestSettings = AccessPackageAutomaticRequestSettings()
automaticRequestSettings.requestAccessForAllowedTargets = true


request_body.automaticRequestSettings = automaticRequestSettings
accessPackage = AccessPackage()
accessPackage.id = '8a36831e-1527-4b2b-aff2-81259a8d8e76'


request_body.accessPackage = accessPackage


request_configuration = AssignmentPoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body = request_body)


```