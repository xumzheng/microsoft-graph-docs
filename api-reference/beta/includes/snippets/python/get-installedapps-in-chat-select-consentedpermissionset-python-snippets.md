---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamsAppInstallationRequestBuilderGetRequestConfiguration(
request_configuration = TeamsAppInstallationRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsAppInstallationRequestBuilderGetQueryParameters()
query_params['select'] = ["consentedPermissionSet","id"]

)
query_params = TeamsAppInstallationRequestBuilderGetQueryParameters()
query_params['select'] = ["consentedPermissionSet","id"]

)


result = await client.chats_by_id('chat-id').installedApps_by_id('teamsAppInstallation-id').get(request_configuration)


```