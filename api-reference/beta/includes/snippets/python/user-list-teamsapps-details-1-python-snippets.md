---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserScopeTeamsAppInstallationRequestBuilderGetRequestConfiguration()

query_params = UserScopeTeamsAppInstallationRequestBuilderGetQueryParameters()
query_params.expand = ["teamsAppDefinition"]

request_config.queryParameters = query_params


result = await client.usersby_id('user-id')_teamwork_installedAppsby_id('userScopeTeamsAppInstallation-id').get(request_config)


```