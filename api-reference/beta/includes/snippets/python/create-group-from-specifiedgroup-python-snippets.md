---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/odata/groups(\'dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef\')');



graphServiceClient.policies().mobileDeviceManagementPoliciesById('mobilityManagementPolicy-id').includedGroups().ref().post(requestBody);


```