---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = InstalledAppsRequestBuilder.InstalledAppsRequestBuilderGetQueryParameters(
				expand = ["teamsAppDefinition($expand=bot)"],
)

request_configuration = InstalledAppsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.users_by_id('user-id').teamwork.installedApps.get(request_configuration = request_configuration)


```