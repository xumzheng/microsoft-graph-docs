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


result = await client.onPremisesPublishingProfilesby_id('onPremisesPublishingProfile-id').publishedResourcesby_id('publishedResource-id').get(request_config)


```