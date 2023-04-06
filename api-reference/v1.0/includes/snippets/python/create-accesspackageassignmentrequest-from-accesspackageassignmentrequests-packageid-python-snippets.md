---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentRequest()
request_body.setRequestType(AccessPackageRequestType('useradd'))

assignment = AccessPackageAssignment()
additionalData = [
'accessPackageId' => 'd7be3253-b9c6-4fab-adef-30d30de8da2b', 
];
assignment.setAdditionalData(additionalData)



request_body.setAssignment($assignment)

request_config = AssignmentRequestsRequestBuilderPostRequestConfiguration(
request_config = AssignmentRequestsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identityGovernance.entitlementManagement.assignmentRequests.post(request_body, headers=)


```