---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(
request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params['expand'] = ["appDefinitions($select=id,displayName,allowedInstallationScopes)"]
query_params['filter'] = "appDefinitions/any"

)
query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params['expand'] = ["appDefinitions($select=id,displayName,allowedInstallationScopes)"]
query_params['filter'] = "appDefinitions/any"

)


result = await client.appCatalogs.teamsApps.get(request_configuration)


```