---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = SitesRequestBuilderGetRequestConfiguration(
request_config = SitesRequestBuilderGetRequestConfiguration(query_params=query_params = SitesRequestBuilderGetQueryParameters()
query_params.select = ["siteCollection","webUrl"]
query_params.filter = "siteCollection/root ne null"

)
query_params = SitesRequestBuilderGetQueryParameters()
query_params.select = ["siteCollection","webUrl"]
query_params.filter = "siteCollection/root ne null"

)


result = await client.sites.get(request_config, headers=request_config)


```