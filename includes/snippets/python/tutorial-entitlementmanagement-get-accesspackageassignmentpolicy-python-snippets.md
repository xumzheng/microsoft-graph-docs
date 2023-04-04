---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageAssignmentPolicy();
request_body.setAccessPackageId('88203d16-0e31-41d4-87b2-dd402f1435e9');

request_body.setDisplayName('Specific users');

request_body.setDescription('Specific users can request assignment');

request_body.setAccessReviewSettings(null);

request_body.setDurationInDays(30);

requestorSettings = RequestorSettings();
requestorSettings.setScopeType('SpecificDirectorySubjects');

requestorSettings.setAcceptRequests(true);

allowedRequestorsUserSet1 = UserSet();
allowedRequestorsUserSet1.set@odatatype('#microsoft.graph.singleUser');

allowedRequestorsUserSet1.setIsBackup(false);

additionalData = [
'id' => '007d1c7e-7fa8-4e33-b678-5e437acdcddc', 
'description' => 'Requestor1', 
];
allowedRequestorsUserSet1.setAdditionalData(additionalData);



allowedRequestorsArray []= allowedRequestorsUserSet1;
requestorSettings.setAllowedRequestors(allowedRequestorsArray);



request_body.setRequestorSettings($requestorSettings);
requestApprovalSettings = ApprovalSettings();
requestApprovalSettings.setIsApprovalRequired(false);

requestApprovalSettings.setIsApprovalRequiredForExtension(false);

requestApprovalSettings.setIsRequestorJustificationRequired(false);

requestApprovalSettings.setApprovalMode('NoApproval');

requestApprovalSettings.setApprovalStages([]);


request_body.setRequestApprovalSettings($requestApprovalSettings);


result = await client.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies().post(request_body);


```