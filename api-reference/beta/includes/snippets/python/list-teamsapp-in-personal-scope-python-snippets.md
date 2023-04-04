---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = TeamsAppsRequestBuilderGetRequestConfiguration()

query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params.expand = ["appDefinitions($select=id,displayName,allowedInstallationScopes)"]
query_params.filter = "appDefinitions/any"

request_config.queryParameters = query_params


result = await client.appCatalogs.teamsApps.get(request_config)


```