---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = HealthOverviewsRequestBuilder.HealthOverviewsRequestBuilderGetQueryParameters(
				expand = ["issues"],
)

request_configuration = HealthOverviewsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.admin.serviceAnnouncement.healthOverviews.get(request_configuration = request_configuration)


```