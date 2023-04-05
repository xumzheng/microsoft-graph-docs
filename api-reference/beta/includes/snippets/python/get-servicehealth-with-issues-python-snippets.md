---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ServiceHealthRequestBuilderGetRequestConfiguration(
query_params = ServiceHealthRequestBuilderGetQueryParameters()
query_params.expand = ["issues"]

)


result = await client.admin.serviceAnnouncement.healthOverviews_by_id('serviceHealth-id').get(request_config)


```