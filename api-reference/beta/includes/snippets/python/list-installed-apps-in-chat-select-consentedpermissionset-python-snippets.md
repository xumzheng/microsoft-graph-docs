---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = InstalledAppsRequestBuilderGetRequestConfiguration(
query_params = InstalledAppsRequestBuilderGetQueryParameters()
query_params.select = ["consentedPermissionSet","id"]

)


result = await client.chats_by_id('chat-id').installedApps.get(request_config)


```