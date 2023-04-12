---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.id = '87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187'

request_body.displayName = 'All Users'

request_body.description = 'All users can request for access to the directory.'

request_body.AllowedTargetScope(AllowedTargetScope('alldirectoryusers'))

request_body.automaticRequestSettings=null

request_body.SpecificAllowedTargets([])

expiration = ExpirationPattern()
expiration.Type(ExpirationPatternType('noexpiration'))


request_body.expiration = expiration
requestorSettings = AccessPackageAssignmentRequestorSettings()
requestorSettings.enableTargetsToSelfAddAccess = true

requestorSettings.enableTargetsToSelfUpdateAccess = false

requestorSettings.enableTargetsToSelfRemoveAccess = true

requestorSettings.allowCustomAssignmentSchedule = false

requestorSettings.enableOnBehalfRequestorsToAddAccess = false

requestorSettings.enableOnBehalfRequestorsToUpdateAccess = false

requestorSettings.enableOnBehalfRequestorsToRemoveAccess = false

requestorSettings.OnBehalfRequestors([])


request_body.requestorSettings = requestorSettings
requestApprovalSettings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.isApprovalRequiredForAdd = true

requestApprovalSettings.isApprovalRequiredForUpdate = false

stagesAccessPackageApprovalStage1 = AccessPackageApprovalStage()
stagesAccessPackageApprovalStage1.durationbeforeautomaticdenial =  \DateInterval('P2D')

stagesAccessPackageApprovalStage1.isApproverJustificationRequired = false

stagesAccessPackageApprovalStage1.isEscalationEnabled = false

stagesAccessPackageApprovalStage1.durationbeforeescalation =  \DateInterval('PT0S')

primaryApproversSubjectSet1 = SubjectSet()
primaryApproversSubjectSet1.@odatatype = '#microsoft.graph.requestorManager'

additionalData = [
'managerLevel' => 1,
];
primaryApproversSubjectSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.primaryapprovers(primaryApproversArray)


fallbackPrimaryApproversSubjectSet1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.@odatatype = '#microsoft.graph.singleUser'

additionalData = [
'userId' => 'e6bf4d7d-6824-4dd0-809d-5bf42d4817c2', 
'description' => 'user', 
];
fallbackPrimaryApproversSubjectSet1.additionaldata(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.fallbackprimaryapprovers(fallbackPrimaryApproversArray)


stagesAccessPackageApprovalStage1.EscalationApprovers([])

stagesAccessPackageApprovalStage1.FallbackEscalationApprovers([])


stagesArray []= stagesAccessPackageApprovalStage1;
requestApprovalSettings.stages(stagesArray)



request_body.requestApprovalSettings = requestApprovalSettings
accessPackage = AccessPackage()
accessPackage.id = '49d2c59b-0a81-463d-a8ec-ddad3935d8a0'


request_body.accessPackage = accessPackage



result = await client.identityGovernance.entitlementManagement.assignmentPolicies_by_id('accessPackageAssignmentPolicy-id').put(request_body = request_body)


```