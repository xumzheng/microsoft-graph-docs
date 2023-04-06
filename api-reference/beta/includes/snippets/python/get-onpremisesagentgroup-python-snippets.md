---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = OnPremisesAgentGroupRequestBuilderGetRequestConfiguration(
request_configuration = OnPremisesAgentGroupRequestBuilderGetRequestConfiguration(query_params=query_params = OnPremisesAgentGroupRequestBuilderGetQueryParameters()
query_params['expand'] = ["publishedResources","agents"]

)
query_params = OnPremisesAgentGroupRequestBuilderGetQueryParameters()
query_params['expand'] = ["publishedResources","agents"]

)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agentGroups_by_id('onPremisesAgentGroup-id').get(request_configuration)


```