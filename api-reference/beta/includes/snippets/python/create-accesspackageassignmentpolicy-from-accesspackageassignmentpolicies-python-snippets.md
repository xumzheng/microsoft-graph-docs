---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.accessPackageId = '56ff43fd-6b05-48df-9634-956a777fce6d'

request_body.displayName = 'direct'

request_body.description = 'direct assignments by administrator'

request_body.accessReviewSettings=null

requestorSettings = RequestorSettings()
requestorSettings.scopeType = 'NoSubjects'

requestorSettings.acceptRequests = true

requestorSettings.AllowedRequestors([])


request_body.requestorSettings = requestorSettings
requestApprovalSettings = ApprovalSettings()
requestApprovalSettings.isApprovalRequired = false

requestApprovalSettings.isApprovalRequiredForExtension = false

requestApprovalSettings.isRequestorJustificationRequired = false

requestApprovalSettings.approvalMode = 'NoApproval'

requestApprovalSettings.ApprovalStages([])


request_body.requestApprovalSettings = requestApprovalSettings


request_configuration = AccessPackageAssignmentPoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```