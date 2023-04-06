---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = InstalledAppsRequestBuilderGetRequestConfiguration(
request_config = InstalledAppsRequestBuilderGetRequestConfiguration(query_params=query_params = InstalledAppsRequestBuilderGetQueryParameters()
query_params.expand = ["teamsAppDefinition"]

)
query_params = InstalledAppsRequestBuilderGetQueryParameters()
query_params.expand = ["teamsAppDefinition"]

)


result = await client.teams_by_id('team-id').installedApps.get(request_config, headers=request_config)


```