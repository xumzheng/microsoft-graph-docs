---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration(
request_config = OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["publishedResources","agents","agentGroups"]
)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').get(request_config, headers=request_config)


```