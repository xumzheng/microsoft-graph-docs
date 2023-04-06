---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.setRequestType('AdminAdd')

accessPackageAssignment = AccessPackageAssignment()
accessPackageAssignment.setTargetId('46184453-e63b-4f20-86c2-c557ed5d5df9')

accessPackageAssignment.setAssignmentPolicyId('2264bf65-76ba-417b-a27d-54d291f0cbc8')

accessPackageAssignment.setAccessPackageId('a914b616-e04e-476b-aa37-91038f0b165b')


request_body.setAccessPackageAssignment($accessPackageAssignment)

request_config = AccessPackageAssignmentRequestsRequestBuilderPostRequestConfiguration(
request_config = AccessPackageAssignmentRequestsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(request_body, headers=)


```