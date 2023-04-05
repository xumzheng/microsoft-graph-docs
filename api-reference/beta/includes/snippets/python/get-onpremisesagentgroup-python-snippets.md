---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OnPremisesAgentGroupRequestBuilderGetRequestConfiguration(
query_params = OnPremisesAgentGroupRequestBuilderGetQueryParameters()
query_params.expand = ["publishedResources","agents"]

)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agentGroups_by_id('onPremisesAgentGroup-id').get(request_config)


```