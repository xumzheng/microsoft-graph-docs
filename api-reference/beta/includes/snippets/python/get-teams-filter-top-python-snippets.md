---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamsRequestBuilderGetRequestConfiguration(
request_configuration = TeamsRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsRequestBuilderGetQueryParameters()
query_params['filter'] = "startswith(displayName,%20'A')"
query_params['top'] = 2

)
query_params = TeamsRequestBuilderGetQueryParameters()
query_params['filter'] = "startswith(displayName,%20'A')"
query_params['top'] = 2

)


await client.teams.get(request_configuration)


```