---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ItemsRequestBuilderGetRequestConfiguration()

query_params = ItemsRequestBuilderGetQueryParameters()
query_params.expand = ["fields(select=Name,Color,Quantity)"]

request_config.queryParameters = query_params


result = await client.sitesby_id('site-id')_listsby_id('list-id')_items.get(request_config)


```