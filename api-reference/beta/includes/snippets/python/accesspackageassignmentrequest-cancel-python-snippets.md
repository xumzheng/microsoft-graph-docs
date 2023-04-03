---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CancelPostRequestBody();
additionalData = [
'id' => 'request-id', 
'requestStatus' => 'cancelled', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.identityGovernance().entitlementManagement().accessPackageAssignmentRequestsById('accessPackageAssignmentRequest-id').cancel().post(requestBody);


```