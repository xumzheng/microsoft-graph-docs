---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ChangeScreenSharingRolePostRequestBody();
requestBody.setRole(ScreenSharingRole('viewer'));



awaitclient.communications().callsById('call-id').changeScreenSharingRole().post(requestBody);


```