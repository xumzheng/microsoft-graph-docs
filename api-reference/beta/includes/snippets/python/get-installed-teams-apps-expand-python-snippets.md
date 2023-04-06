---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamsAppInstallationRequestBuilderGetRequestConfiguration(
request_configuration = TeamsAppInstallationRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsAppInstallationRequestBuilderGetQueryParameters()
query_params['expand'] = ["teamsAppDefinition"]

)
query_params = TeamsAppInstallationRequestBuilderGetQueryParameters()
query_params['expand'] = ["teamsAppDefinition"]

)


result = await client.teams_by_id('team-id').installedApps_by_id('teamsAppInstallation-id').get(request_configuration)


```