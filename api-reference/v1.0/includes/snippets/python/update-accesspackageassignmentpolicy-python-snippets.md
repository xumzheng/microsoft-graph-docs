---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.setId('87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187')

request_body.setDisplayName('All Users')

request_body.setDescription('All users can request for access to the directory.')

request_body.setAllowedTargetScope(AllowedTargetScope('alldirectoryusers'))

request_body.setAutomaticRequestSettings(null)

request_body.setSpecificAllowedTargets([])

expiration = ExpirationPattern()
expiration.setType(ExpirationPatternType('noexpiration'))


request_body.setExpiration($expiration)
requestorSettings = AccessPackageAssignmentRequestorSettings()
requestorSettings.setEnableTargetsToSelfAddAccess(true)

requestorSettings.setEnableTargetsToSelfUpdateAccess(false)

requestorSettings.setEnableTargetsToSelfRemoveAccess(true)

requestorSettings.setAllowCustomAssignmentSchedule(false)

requestorSettings.setEnableOnBehalfRequestorsToAddAccess(false)

requestorSettings.setEnableOnBehalfRequestorsToUpdateAccess(false)

requestorSettings.setEnableOnBehalfRequestorsToRemoveAccess(false)

requestorSettings.setOnBehalfRequestors([])


request_body.setRequestorSettings($requestorSettings)
requestApprovalSettings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.setIsApprovalRequiredForAdd(true)

requestApprovalSettings.setIsApprovalRequiredForUpdate(false)

stagesAccessPackageApprovalStage1 = AccessPackageApprovalStage()
$stagesAccessPackageApprovalStage1.setDurationBeforeAutomaticDenial( \DateInterval('P2D'))

stagesAccessPackageApprovalStage1.setIsApproverJustificationRequired(false)

stagesAccessPackageApprovalStage1.setIsEscalationEnabled(false)

$stagesAccessPackageApprovalStage1.setDurationBeforeEscalation( \DateInterval('PT0S'))

primaryApproversSubjectSet1 = SubjectSet()
primaryApproversSubjectSet1.set@odatatype('#microsoft.graph.requestorManager')

additionalData = [
'managerLevel' => 1,
];
primaryApproversSubjectSet1.setAdditionalData(additionalData)



primaryApproversArray []= primaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.setPrimaryApprovers(primaryApproversArray)


fallbackPrimaryApproversSubjectSet1 = SubjectSet()
fallbackPrimaryApproversSubjectSet1.set@odatatype('#microsoft.graph.singleUser')

additionalData = [
'userId' => 'e6bf4d7d-6824-4dd0-809d-5bf42d4817c2', 
'description' => 'user', 
];
fallbackPrimaryApproversSubjectSet1.setAdditionalData(additionalData)



fallbackPrimaryApproversArray []= fallbackPrimaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.setFallbackPrimaryApprovers(fallbackPrimaryApproversArray)


stagesAccessPackageApprovalStage1.setEscalationApprovers([])

stagesAccessPackageApprovalStage1.setFallbackEscalationApprovers([])


stagesArray []= stagesAccessPackageApprovalStage1;
requestApprovalSettings.setStages(stagesArray)



request_body.setRequestApprovalSettings($requestApprovalSettings)
accessPackage = AccessPackage()
accessPackage.setId('49d2c59b-0a81-463d-a8ec-ddad3935d8a0')


request_body.setAccessPackage($accessPackage)


result = await client.identityGovernance.entitlementManagement.assignmentPolicies_by_id('accessPackageAssignmentPolicy-id').put(request_body, headers=)


```