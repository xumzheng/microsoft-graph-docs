---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.requestType = 'AdminAdd'

access_package_assignment = AccessPackageAssignment()
accessPackageAssignment.targetId = '46184453-e63b-4f20-86c2-c557ed5d5df9'

accessPackageAssignment.assignmentPolicyId = '2264bf65-76ba-417b-a27d-54d291f0cbc8'

accessPackageAssignment.accessPackageId = 'a914b616-e04e-476b-aa37-91038f0b165b'


request_body.access_package_assignment = accessPackageAssignment



result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(request_body = request_body)


```