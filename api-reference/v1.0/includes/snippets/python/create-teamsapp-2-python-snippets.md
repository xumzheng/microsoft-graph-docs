---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TeamsAppsRequestBuilderPostRequestConfiguration()

query_params = TeamsAppsRequestBuilderPostQueryParameters()
query_params.requiresreview = true

request_config.queryParameters = query_params


await client.appCatalogs.teamsApps.post(request_config)


```