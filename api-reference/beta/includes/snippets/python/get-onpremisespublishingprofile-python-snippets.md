---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration()

query_params = OnPremisesPublishingProfileRequestBuilderGetQueryParameters()
query_params.expand = ["publishedResources","agents","agentGroups"]

request_config.queryParameters = query_params


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').get(request_config)


```