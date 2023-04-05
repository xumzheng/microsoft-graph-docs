---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PublishedResourceRequestBuilderGetRequestConfiguration()

query_params = PublishedResourceRequestBuilderGetQueryParameters()
query_params.expand = ["agentGroups"]

request_config.queryParameters = query_params


result = await client.onPremisesPublishingProfiles._by_id('onPremisesPublishingProfile-id').publishedResources._by_id('publishedResource-id').get(request_config)


```