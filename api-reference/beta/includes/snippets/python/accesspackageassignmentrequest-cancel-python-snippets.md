---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CancelPostRequestBody()
additionalData = [
'id' => 'request-id', 
'requestStatus' => 'cancelled', 
];
request_body.setAdditionalData(additionalData)




await client.identityGovernance.entitlementManagement.accessPackageAssignmentRequests_by_id('accessPackageAssignmentRequest-id').cancel.post(request_body)


```