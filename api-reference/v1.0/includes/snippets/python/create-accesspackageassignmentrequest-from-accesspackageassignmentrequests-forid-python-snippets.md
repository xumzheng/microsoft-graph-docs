---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.RequestType(AccessPackageRequestType('adminremove'))

assignment = AccessPackageAssignment()
assignment.id = 'a6bb6942-3ae1-4259-9908-0133aaee9377'


request_body.assignment = assignment


request_configuration = AssignmentRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.assignmentRequests.post(request_body = request_body)


```