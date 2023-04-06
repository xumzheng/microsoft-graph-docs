---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OnPremisesAgentRequestBuilderGetRequestConfiguration(
request_config = OnPremisesAgentRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["agentGroups"]
)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agents_by_id('onPremisesAgent-id').get(request_config, headers=request_config)


```