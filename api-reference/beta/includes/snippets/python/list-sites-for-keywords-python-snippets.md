---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = SitesRequestBuilderGetRequestConfiguration();

query_params = SitesRequestBuilderGetQueryParameters();
query_params.select = ["siteCollection","webUrl"];
query_params.filter = "siteCollection/root ne null";

request_config.queryParameters = query_params;


result = awaitclient.sites().get(request_config);


```