---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = OnPremisesAgentGroupRequestBuilder.OnPremisesAgentGroupRequestBuilderGetQueryParameters(
				expand = ["publishedResources","agents"],
)

request_configuration = OnPremisesAgentGroupRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agentGroups_by_id('onPremisesAgentGroup-id').get(request_configuration = request_configuration)


```