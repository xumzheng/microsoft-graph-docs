---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = InstalledAppsRequestBuilderGetRequestConfiguration(
request_configuration = InstalledAppsRequestBuilderGetRequestConfiguration(query_params=query_params = InstalledAppsRequestBuilderGetQueryParameters()
query_params['expand'] = ["teamsApp","teamsAppDefinition"]
query_params['filter'] = "teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'"

)
query_params = InstalledAppsRequestBuilderGetQueryParameters()
query_params['expand'] = ["teamsApp","teamsAppDefinition"]
query_params['filter'] = "teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'"

)


result = await client.teams_by_id('team-id').installedApps.get(request_configuration)


```