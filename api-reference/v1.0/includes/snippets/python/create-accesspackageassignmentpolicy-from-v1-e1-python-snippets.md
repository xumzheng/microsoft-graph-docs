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
requestor_settings = AccessPackageAssignmentRequestorSettings()
requestorSettings.enable_targets_to_self_add_access = False

requestorSettings.enable_targets_to_self_update_access = False

requestorSettings.enable_targets_to_self_remove_access = False

requestorSettings.allow_custom_assignment_schedule = True

requestorSettings.enable_on_behalf_requestors_to_add_access = False

requestorSettings.enable_on_behalf_requestors_to_update_access = False

requestorSettings.enable_on_behalf_requestors_to_remove_access = False

requestorSettings.OnBehalfRequestors([])


request_body.requestor_settings = requestorSettings
request_approval_settings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.is_approval_required_for_add = False

requestApprovalSettings.is_approval_required_for_update = False

requestApprovalSettings.Stages([])


request_body.request_approval_settings = requestApprovalSettings
access_package = AccessPackage()
accessPackage.id = 'a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b'


request_body.access_package = accessPackage



result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body = request_body)


```