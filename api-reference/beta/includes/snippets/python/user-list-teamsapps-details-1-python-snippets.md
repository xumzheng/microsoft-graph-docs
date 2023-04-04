---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = UserScopeTeamsAppInstallationRequestBuilderGetRequestConfiguration()

query_params = UserScopeTeamsAppInstallationRequestBuilderGetQueryParameters()
query_params.expand = ["teamsAppDefinition"]

request_config.queryParameters = query_params


result = await client.usersById('user-id').teamwork.installedAppsById('userScopeTeamsAppInstallation-id').get(request_config)


```