---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ChangeScreenSharingRolePostRequestBody();
requestBody.setRole(ScreenSharingRole('viewer'));



graphServiceClient.communications().callsById('call-id').changeScreenSharingRole().post(requestBody);


```