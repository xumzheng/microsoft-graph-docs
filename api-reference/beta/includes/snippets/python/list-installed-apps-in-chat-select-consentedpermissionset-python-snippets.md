---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = InstalledAppsRequestBuilder.InstalledAppsRequestBuilderGetQueryParameters(
		select = ["consentedPermissionSet","id"],
)

request_configuration = InstalledAppsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.chats_by_id('chat-id').installedApps.get(request_configuration = request_configuration)


```