---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TeamsAppsRequestBuilderGetRequestConfiguration(
request_config = TeamsAppsRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params.filter = "id eq '876df28f-2e78-423b-94a5-44181bd0e225'"
query_params.expand = ["appDefinitions"]

)
query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params.filter = "id eq '876df28f-2e78-423b-94a5-44181bd0e225'"
query_params.expand = ["appDefinitions"]

)


result = await client.appCatalogs.teamsApps.get(request_config, headers=request_config)


```