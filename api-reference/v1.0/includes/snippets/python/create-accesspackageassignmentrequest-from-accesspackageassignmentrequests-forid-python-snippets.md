---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageAssignmentRequest()
request_body.setRequestType(AccessPackageRequestType('adminremove'))

assignment = AccessPackageAssignment()
assignment.setId('a6bb6942-3ae1-4259-9908-0133aaee9377')


request_body.setAssignment($assignment)


result = await client.identityGovernance.entitlementManagement.assignmentRequests.post(request_body)


```