---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageAssignmentRequest();
requestBody.setRequestType('AdminRemove');

accessPackageAssignment = AccessPackageAssignment();
accessPackageAssignment.setId('a6bb6942-3ae1-4259-9908-0133aaee9377');


requestBody.setAccessPackageAssignment($accessPackageAssignment);


result = awaitclient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests().post(requestBody);


```