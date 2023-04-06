---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = OnPremisesAgentRequestBuilderGetRequestConfiguration(
request_configuration = OnPremisesAgentRequestBuilderGetRequestConfiguration(query_params=query_params = OnPremisesAgentRequestBuilderGetQueryParameters()
query_params['expand'] = ["agentGroups"]

)
query_params = OnPremisesAgentRequestBuilderGetQueryParameters()
query_params['expand'] = ["agentGroups"]

)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agents_by_id('onPremisesAgent-id').get(request_configuration)


```