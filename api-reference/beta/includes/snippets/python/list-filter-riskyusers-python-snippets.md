---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RiskyUsersRequestBuilderGetRequestConfiguration(
request_configuration = RiskyUsersRequestBuilderGetRequestConfiguration(query_params=query_params = RiskyUsersRequestBuilderGetQueryParameters()
query_params['filter'] = "riskLevel eq microsoft.graph.riskLevel'medium'"

)
query_params = RiskyUsersRequestBuilderGetQueryParameters()
query_params['filter'] = "riskLevel eq microsoft.graph.riskLevel'medium'"

)


result = await client.identityProtection.riskyUsers.get(request_configuration)


```