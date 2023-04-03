---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AccessPackageAssignmentRequest();
requestBody.setRequestType(AccessPackageRequestType('adminremove'));

assignment = AccessPackageAssignment();
assignment.setId('a6bb6942-3ae1-4259-9908-0133aaee9377');


requestBody.setAssignment($assignment);


result = await client.identityGovernance().entitlementManagement().assignmentRequests().post(requestBody);


```