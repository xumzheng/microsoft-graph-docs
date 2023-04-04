---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = SitesRequestBuilderGetRequestConfiguration();

query_params = SitesRequestBuilderGetQueryParameters;
query_params.search = "{query}";

request_config.queryParameters = query_params;


result = await client.sites().get(request_config);


```