---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(
request_configuration = TeamsAppsRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params['filter'] = "distributionMethod eq 'organization'"

)
query_params = TeamsAppsRequestBuilderGetQueryParameters()
query_params['filter'] = "distributionMethod eq 'organization'"

)


result = await client.appCatalogs.teamsApps.get(request_configuration)


```