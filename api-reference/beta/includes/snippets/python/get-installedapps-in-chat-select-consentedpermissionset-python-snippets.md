---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = TeamsAppInstallationRequestBuilder.TeamsAppInstallationRequestBuilderGetQueryParameters(
		select = ["consentedPermissionSet","id"],
)

request_configuration = TeamsAppInstallationRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.chats_by_id('chat-id').installedApps_by_id('teamsAppInstallation-id').get(request_configuration = request_configuration)


```