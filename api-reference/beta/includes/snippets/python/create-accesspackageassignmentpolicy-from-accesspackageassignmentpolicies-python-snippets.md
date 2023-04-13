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

requestor_settings = RequestorSettings()
requestorSettings.scopeType = 'NoSubjects'

requestorSettings.accept_requests = True

requestorSettings.AllowedRequestors([])


request_body.requestor_settings = requestorSettings
request_approval_settings = ApprovalSettings()
requestApprovalSettings.is_approval_required = False

requestApprovalSettings.is_approval_required_for_extension = False

requestApprovalSettings.is_requestor_justification_required = False

requestApprovalSettings.approvalMode = 'NoApproval'

requestApprovalSettings.ApprovalStages([])


request_body.request_approval_settings = requestApprovalSettings



result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```