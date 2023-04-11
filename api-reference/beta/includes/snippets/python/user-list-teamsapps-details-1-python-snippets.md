---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UserScopeTeamsAppInstallationRequestBuilder.UserScopeTeamsAppInstallationRequestBuilderGetQueryParameters(
				expand = ["teamsAppDefinition"],
)

request_configuration = UserScopeTeamsAppInstallationRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.users_by_id('user-id').teamwork.installedApps_by_id('userScopeTeamsAppInstallation-id').get(request_configuration = request_configuration)


```