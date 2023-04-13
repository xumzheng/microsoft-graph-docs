---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.accessPackageId = '88203d16-0e31-41d4-87b2-dd402f1435e9'

request_body.displayName = 'Specific users'

request_body.description = 'Specific users can request assignment'

request_body.accessReviewSettings=null

request_body.duration_in_days = 30

requestor_settings = RequestorSettings()
requestorSettings.scopeType = 'SpecificDirectorySubjects'

requestorSettings.accept_requests = True

allowed_requestors_user_set1 = UserSet()
allowedRequestorsUserSet1.@odatatype = '#microsoft.graph.singleUser'

allowedRequestorsUserSet1.is_backup = False

additionalData = [
'id' => '007d1c7e-7fa8-4e33-b678-5e437acdcddc', 
'description' => 'Requestor1', 
];
allowedRequestorsUserSet1.additionaldata(additionalData)



allowedRequestorsArray []= allowedRequestorsUserSet1;
requestorSettings.allowedrequestors(allowedRequestorsArray)



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