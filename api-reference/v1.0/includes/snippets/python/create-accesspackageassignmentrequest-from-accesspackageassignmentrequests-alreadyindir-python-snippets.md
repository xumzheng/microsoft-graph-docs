---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageAssignmentRequest();
request_body.setRequestType(AccessPackageRequestType('adminadd'));

assignment = AccessPackageAssignment();
additionalData = [
'targetId' => '46184453-e63b-4f20-86c2-c557ed5d5df9', 
'assignmentPolicyId' => '2264bf65-76ba-417b-a27d-54d291f0cbc8', 
'accessPackageId' => 'a914b616-e04e-476b-aa37-91038f0b165b', 
];
assignment.setAdditionalData(additionalData);



request_body.setAssignment($assignment);


result = await client.identityGovernance.entitlementManagement.assignmentRequests.post(request_body);


```