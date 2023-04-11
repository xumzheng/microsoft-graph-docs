---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.displayName = 'New Policy'

request_body.description = 'policy for assignment'

request_body.AllowedTargetScope(AllowedTargetScope('notspecified'))

request_body.SpecificAllowedTargets([])

expiration = ExpirationPattern()
Expiration.endDateTime=null

Expiration.duration=null

expiration.Type(ExpirationPatternType('noexpiration'))


request_body.expiration = expiration
requestorSettings = AccessPackageAssignmentRequestorSettings()
requestorSettings.enableTargetsToSelfAddAccess = false

requestorSettings.enableTargetsToSelfUpdateAccess = false

requestorSettings.enableTargetsToSelfRemoveAccess = false

requestorSettings.allowCustomAssignmentSchedule = true

requestorSettings.enableOnBehalfRequestorsToAddAccess = false

requestorSettings.enableOnBehalfRequestorsToUpdateAccess = false

requestorSettings.enableOnBehalfRequestorsToRemoveAccess = false

requestorSettings.OnBehalfRequestors([])


request_body.requestorSettings = requestorSettings
requestApprovalSettings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.isApprovalRequiredForAdd = false

requestApprovalSettings.isApprovalRequiredForUpdate = false

requestApprovalSettings.Stages([])


request_body.requestApprovalSettings = requestApprovalSettings
accessPackage = AccessPackage()
accessPackage.id = 'a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b'


request_body.accessPackage = accessPackage



result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body = request_body)


```