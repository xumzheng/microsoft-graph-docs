---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(
request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params['filter'] = "externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'"

)
query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params['filter'] = "externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'"

)


result = await client.appCatalogs.teamsApps.get(request_configuration)


```