---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(
request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params['filter'] = "id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'"

)
query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params['filter'] = "id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'"

)


result = await client.appCatalogs.teamsApps.get(request_configuration)


```