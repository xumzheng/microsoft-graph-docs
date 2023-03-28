---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CancelPostRequestBody();
$additionalData = [
'id' => 'request-id', 
'requestStatus' => 'cancelled', 
];
$requestBody->setAdditionalData($additionalData);




$graphServiceClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentRequestsById('accessPackageAssignmentRequest-id')->cancel()->post($requestBody);


```