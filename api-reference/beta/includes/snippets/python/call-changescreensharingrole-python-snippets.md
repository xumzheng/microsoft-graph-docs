---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChangeScreenSharingRolePostRequestBody()
request_body.setRole(ScreenSharingRole('viewer'))



await client.communications.callsById('call-id').changeScreenSharingRole.post(request_body)


```