---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.setRequestType('UserAdd')

accessPackageAssignment = AccessPackageAssignment()
accessPackageAssignment.setAccessPackageId('a914b616-e04e-476b-aa37-91038f0b165b')


request_body.setAccessPackageAssignment($accessPackageAssignment)
request_body.setJustification('Need access to New Hire access package')


request_config = AccessPackageAssignmentRequestsRequestBuilderPostRequestConfiguration(
request_config = AccessPackageAssignmentRequestsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(request_body, headers=)


```