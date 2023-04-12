---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = PublishedResourcesRequestBuilder.PublishedResourcesRequestBuilderGetQueryParameters(
		expand = ["agentGroups"],
)

request_configuration = PublishedResourcesRequestBuilder.PublishedResourcesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').publishedResources.get(request_configuration = request_configuration)


```