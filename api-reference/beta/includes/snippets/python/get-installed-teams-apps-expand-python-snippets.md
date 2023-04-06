---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TeamsAppInstallationRequestBuilderGetRequestConfiguration(
request_config = TeamsAppInstallationRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["teamsAppDefinition"]
)


result = await client.teams_by_id('team-id').installedApps_by_id('teamsAppInstallation-id').get(request_config, headers=request_config)


```