---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AccessPackageAssignmentRequest();
requestBody.setRequestType('UserAdd');

accessPackageAssignment = AccessPackageAssignment();
accessPackageAssignment.setAccessPackageId('a914b616-e04e-476b-aa37-91038f0b165b');


requestBody.setAccessPackageAssignment($accessPackageAssignment);
requestBody.setJustification('Need access to New Hire access package');



result = await client.identityGovernance().entitlementManagement().accessPackageAssignmentRequests().post(requestBody);


```