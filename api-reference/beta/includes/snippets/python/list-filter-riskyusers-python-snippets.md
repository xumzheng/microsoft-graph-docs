---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = RiskyUsersRequestBuilder.RiskyUsersRequestBuilderGetQueryParameters(
				filter = "riskLevel eq microsoft.graph.riskLevel'medium'",
)

request_configuration = RiskyUsersRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityProtection.riskyUsers.get(request_configuration = request_configuration)


```