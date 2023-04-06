---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AgentsRequestBuilderGetRequestConfiguration(
request_config = AgentsRequestBuilderGetRequestConfiguration(query_params=query_params = AgentsRequestBuilderGetQueryParameters()
query_params.expand = ["agentGroups"]

)
query_params = AgentsRequestBuilderGetQueryParameters()
query_params.expand = ["agentGroups"]

)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agents.get(request_config, headers=request_config)


```