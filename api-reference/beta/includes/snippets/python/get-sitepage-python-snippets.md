---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = SitePageRequestBuilder.SitePageRequestBuilderGetQueryParameters(
				select = ["id","title"],
				expand = ["webparts"],
)

request_configuration = SitePageRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').get(request_configuration = request_configuration)


```