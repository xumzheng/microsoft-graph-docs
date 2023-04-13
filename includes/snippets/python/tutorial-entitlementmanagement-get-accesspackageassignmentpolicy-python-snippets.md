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

request_body.durationInDays = 30

requestorSettings = RequestorSettings()
requestorSettings.scopeType = 'SpecificDirectorySubjects'

requestorSettings.acceptRequests = true

allowedRequestorsUserSet1 = UserSet()
allowedRequestorsUserSet1.@odatatype = '#microsoft.graph.singleUser'

allowedRequestorsUserSet1.isBackup = false

additionalData = [
'id' => '007d1c7e-7fa8-4e33-b678-5e437acdcddc', 
'description' => 'Requestor1', 
];
allowedRequestorsUserSet1.additionaldata(additionalData)



allowedRequestorsArray []= allowedRequestorsUserSet1;
requestorSettings.allowedrequestors(allowedRequestorsArray)



request_body.requestorSettings = requestorSettings
requestApprovalSettings = ApprovalSettings()
requestApprovalSettings.isApprovalRequired = false

requestApprovalSettings.isApprovalRequiredForExtension = false

requestApprovalSettings.isRequestorJustificationRequired = false

requestApprovalSettings.approvalMode = 'NoApproval'

requestApprovalSettings.ApprovalStages([])


request_body.requestApprovalSettings = requestApprovalSettings



result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```