---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AuthorizationPolicy();
additionalData = [
'guestUserRole' => '2af84b1e-32c8-42b7-82bc-daa82404023b', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.policies().authorizationPolicyById('authorizationPolicy-id').patch(requestBody);


```