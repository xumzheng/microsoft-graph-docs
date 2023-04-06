---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ItemsRequestBuilderGetRequestConfiguration(
request_config = ItemsRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["fields(select=Name,Color,Quantity)"]
)


result = await client.sites_by_id('site-id').lists_by_id('list-id').items.get(request_config, headers=request_config)


```