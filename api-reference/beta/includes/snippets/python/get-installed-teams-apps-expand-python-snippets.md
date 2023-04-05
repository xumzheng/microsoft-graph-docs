---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TeamsAppInstallationRequestBuilderGetRequestConfiguration()

query_params = TeamsAppInstallationRequestBuilderGetQueryParameters()
query_params.expand = ["teamsAppDefinition"]

request_config.queryParameters = query_params


result = await client.teams._by_id('team-id').installedApps._by_id('teamsAppInstallation-id').get(request_config)


```