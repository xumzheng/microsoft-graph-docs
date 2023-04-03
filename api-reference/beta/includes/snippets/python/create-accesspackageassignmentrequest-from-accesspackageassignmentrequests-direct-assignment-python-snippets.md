---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageAssignmentRequest();
requestBody.setRequestType('AdminAdd');

accessPackageAssignment = AccessPackageAssignment();
accessPackageAssignmentTarget = AccessPackageSubject();
accessPackageAssignmentTarget.setEmail('user@contoso.com');


accessPackageAssignment.setTarget($accessPackageAssignmentTarget);
accessPackageAssignment.setAssignmentPolicyId('2264bf65-76ba-417b-a27d-54d291f0cbc8');

accessPackageAssignment.setAccessPackageId('a914b616-e04e-476b-aa37-91038f0b165b');


requestBody.setAccessPackageAssignment($accessPackageAssignment);


requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests().post(requestBody);


```