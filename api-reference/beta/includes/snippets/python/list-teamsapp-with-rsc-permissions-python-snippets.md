---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TeamsAppsRequestBuilderGetRequestConfiguration(
query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params.filter = "id eq 'a5228c26-a9ae-4702-90e0-79a5246d2f7d'"
query_params.expand = ["appDefinitions($select=id,authorization)"]

)


result = await client.appCatalogs.teamsApps.get(request_config)


```