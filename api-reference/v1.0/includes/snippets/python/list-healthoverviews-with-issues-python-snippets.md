---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = HealthOverviewsRequestBuilderGetRequestConfiguration();

query_params = HealthOverviewsRequestBuilderGetQueryParameters();
query_params.expand = ["issues"];

request_config.queryParameters = query_params;


result = awaitclient.admin().serviceAnnouncement().healthOverviews().get(request_config);


```