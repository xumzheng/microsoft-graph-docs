---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AccessPackageAssignmentRequest();
requestBody.setRequestType(AccessPackageRequestType('useradd'));

assignment = AccessPackageAssignment();
additionalData = [
'accessPackageId' => 'd7be3253-b9c6-4fab-adef-30d30de8da2b', 
];
assignment.setAdditionalData(additionalData);



requestBody.setAssignment($assignment);


result = await client.identityGovernance().entitlementManagement().assignmentRequests().post(requestBody);


```