---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = TeamsAppsRequestBuilder.TeamsAppsRequestBuilderGetQueryParameters(
		expand = ["appDefinitions($select=id,displayName,allowedInstallationScopes)"],
		filter = "appDefinitions/any",
)

request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.appCatalogs.teamsApps.get(request_configuration = request_configuration)


```