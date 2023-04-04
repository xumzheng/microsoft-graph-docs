---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageAssignmentPolicy()
request_body.setDisplayName('New Policy')

request_body.setDescription('policy for assignment')

request_body.setAllowedTargetScope(AllowedTargetScope('notspecified'))

request_body.setSpecificAllowedTargets([])

expiration = ExpirationPattern()
Expiration.setEndDateTime(null)

Expiration.setDuration(null)

expiration.setType(ExpirationPatternType('noexpiration'))


request_body.setExpiration($expiration)
requestorSettings = AccessPackageAssignmentRequestorSettings()
requestorSettings.setEnableTargetsToSelfAddAccess(false)

requestorSettings.setEnableTargetsToSelfUpdateAccess(false)

requestorSettings.setEnableTargetsToSelfRemoveAccess(false)

requestorSettings.setAllowCustomAssignmentSchedule(true)

requestorSettings.setEnableOnBehalfRequestorsToAddAccess(false)

requestorSettings.setEnableOnBehalfRequestorsToUpdateAccess(false)

requestorSettings.setEnableOnBehalfRequestorsToRemoveAccess(false)

requestorSettings.setOnBehalfRequestors([])


request_body.setRequestorSettings($requestorSettings)
requestApprovalSettings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.setIsApprovalRequiredForAdd(false)

requestApprovalSettings.setIsApprovalRequiredForUpdate(false)

requestApprovalSettings.setStages([])


request_body.setRequestApprovalSettings($requestApprovalSettings)
accessPackage = AccessPackage()
accessPackage.setId('a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b')


request_body.setAccessPackage($accessPackage)


result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body)


```