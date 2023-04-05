---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = HealthOverviewsRequestBuilderGetRequestConfiguration()

query_params = HealthOverviewsRequestBuilderGetQueryParameters()
query_params.expand = ["issues"]

request_config.queryParameters = query_params


result = await client.admin_serviceAnnouncement_healthOverviews.get(request_config)


```