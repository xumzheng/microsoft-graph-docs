---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration(
request_configuration = OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration(query_params=query_params = OnPremisesPublishingProfileRequestBuilderGetQueryParameters()
query_params['expand'] = ["publishedResources","agents","agentGroups"]

)
query_params = OnPremisesPublishingProfileRequestBuilderGetQueryParameters()
query_params['expand'] = ["publishedResources","agents","agentGroups"]

)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').get(request_configuration)


```