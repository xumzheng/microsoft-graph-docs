---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.requestType = 'UserAdd'

accessPackageAssignment = AccessPackageAssignment()
accessPackageAssignment.targetId = '007d1c7e-7fa8-4e33-b678-5e437acdcddc'

accessPackageAssignment.assignmentPolicyId = 'db440482-1210-4a60-9b55-3ac7a72f63ba'

accessPackageAssignment.accessPackageId = '88203d16-0e31-41d4-87b2-dd402f1435e9'


request_body.accessPackageAssignment = accessPackageAssignment


request_configuration = AccessPackageAssignmentRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(request_body = request_body)


```