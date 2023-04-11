---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChangeScreenSharingRolePostRequestBody()
request_body.Role(ScreenSharingRole('viewer'))



request_configuration = ChangeScreenSharingRoleRequestBuilderPostRequestConfiguration(
)


await client.communications.calls_by_id('call-id').changeScreenSharingRole.post(request_body = request_body)


```