---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.requestType = 'UserAdd'

accessPackageAssignment = AccessPackageAssignment()
accessPackageAssignment.accessPackageId = 'a914b616-e04e-476b-aa37-91038f0b165b'


request_body.accessPackageAssignment = accessPackageAssignment
request_body.justification = 'Need access to New Hire access package'



request_configuration = AccessPackageAssignmentRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(request_body = request_body)


```