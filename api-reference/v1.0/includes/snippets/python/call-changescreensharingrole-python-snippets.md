---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ChangeScreenSharingRolePostRequestBody();
$requestBody.setRole(new ScreenSharingRole('viewer'));



$graphServiceClient.communications().callsById('call-id').changeScreenSharingRole().post($requestBody);


```