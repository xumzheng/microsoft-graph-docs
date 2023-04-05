---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PublishedResourceRequestBuilderGetRequestConfiguration(
query_params = PublishedResourceRequestBuilderGetQueryParameters()
query_params.expand = ["agentGroups"]

)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').publishedResources_by_id('publishedResource-id').get(request_config)


```