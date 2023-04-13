---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.requestType = 'AdminRemove'

accessPackageAssignment = AccessPackageAssignment()
accessPackageAssignment.id = 'a6bb6942-3ae1-4259-9908-0133aaee9377'


request_body.accessPackageAssignment = accessPackageAssignment



result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(request_body = request_body)


```