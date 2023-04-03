---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ServiceHealthRequestBuilderGetRequestConfiguration();

query_params = ServiceHealthRequestBuilderGetQueryParameters();
query_params.expand = ["issues"];

request_config.queryParameters = query_params;


result = awaitclient.admin().serviceAnnouncement().healthOverviewsById('serviceHealth-id').get(request_config);


```