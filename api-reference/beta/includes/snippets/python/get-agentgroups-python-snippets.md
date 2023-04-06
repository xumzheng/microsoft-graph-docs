---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AgentGroupsRequestBuilderGetRequestConfiguration(
request_configuration = AgentGroupsRequestBuilderGetRequestConfiguration(query_params=query_params = AgentGroupsRequestBuilderGetQueryParameters()
query_params['expand'] = ["agents","publishedResources"]

)
query_params = AgentGroupsRequestBuilderGetQueryParameters()
query_params['expand'] = ["agents","publishedResources"]

)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').agentGroups.get(request_configuration)


```