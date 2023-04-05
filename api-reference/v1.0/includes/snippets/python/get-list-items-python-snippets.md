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


result = await client.sitesById('site-id').listsById('list-id').items.get(request_config)


```