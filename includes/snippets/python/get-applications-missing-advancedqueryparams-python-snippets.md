---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ApplicationsRequestBuilderGetRequestConfiguration();

query_params = ApplicationsRequestBuilderGetQueryParameters();
query_params.search = "\"displayName:Browser\"";

request_config.queryParameters = query_params;


result = awaitclient.applications().get(request_config);


```