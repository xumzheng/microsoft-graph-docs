---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = SitePageRequestBuilderGetRequestConfiguration(
request_configuration = SitePageRequestBuilderGetRequestConfiguration(query_params=query_params = SitePageRequestBuilderGetQueryParameters()
query_params['select'] = ["id","title"]
query_params['expand'] = ["webparts"]

)
query_params = SitePageRequestBuilderGetQueryParameters()
query_params['select'] = ["id","title"]
query_params['expand'] = ["webparts"]

)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').get(request_configuration)


```