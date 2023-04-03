---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CancelPostRequestBody();
additionalData = [
'id' => 'request-id', 
'requestStatus' => 'cancelled', 
];
requestBody.setAdditionalData(additionalData);




await client.identityGovernance().entitlementManagement().accessPackageAssignmentRequestsById('accessPackageAssignmentRequest-id').cancel().post(requestBody);


```