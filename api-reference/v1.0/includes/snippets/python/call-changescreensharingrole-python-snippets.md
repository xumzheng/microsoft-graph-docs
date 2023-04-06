---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChangeScreenSharingRolePostRequestBody()
request_body.setRole(ScreenSharingRole('viewer'))


request_config = ChangeScreenSharingRoleRequestBuilderPostRequestConfiguration(
request_config = ChangeScreenSharingRoleRequestBuilderPostRequestConfiguration(query_params=)


await client.communications.calls_by_id('call-id').changeScreenSharingRole.post(request_body, headers=)


```