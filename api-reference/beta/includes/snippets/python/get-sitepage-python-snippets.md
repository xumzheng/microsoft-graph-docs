---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = SitePageRequestBuilderGetRequestConfiguration(
request_config = SitePageRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id","title"]
params['expand'] = ["webparts"]
)


result = await client.sites_by_id('site-id').pages_by_id('sitePage-id').get(request_config, headers=request_config)


```