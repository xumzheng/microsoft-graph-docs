---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = OnPremisesAgentRequestBuilder.OnPremisesAgentRequestBuilderGetQueryParameters(
				expand = ["agentGroups"],
)

request_configuration = OnPremisesAgentRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agents_by_id('onPremisesAgent-id').get(request_configuration = request_configuration)


```