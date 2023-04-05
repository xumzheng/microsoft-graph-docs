---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.setAccessPackageId('56ff43fd-6b05-48df-9634-956a777fce6d')

request_body.setDisplayName('direct')

request_body.setDescription('direct assignments by administrator')

request_body.setAccessReviewSettings(null)

requestorSettings = RequestorSettings()
requestorSettings.setScopeType('NoSubjects')

requestorSettings.setAcceptRequests(true)

requestorSettings.setAllowedRequestors([])


request_body.setRequestorSettings($requestorSettings)
requestApprovalSettings = ApprovalSettings()
requestApprovalSettings.setIsApprovalRequired(false)

requestApprovalSettings.setIsApprovalRequiredForExtension(false)

requestApprovalSettings.setIsRequestorJustificationRequired(false)

requestApprovalSettings.setApprovalMode('NoApproval')

requestApprovalSettings.setApprovalStages([])


request_body.setRequestApprovalSettings($requestApprovalSettings)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body)


```