---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ItemsRequestBuilderGetRequestConfiguration(
request_configuration = ItemsRequestBuilderGetRequestConfiguration(query_params=query_params = ItemsRequestBuilderGetQueryParameters()
query_params['expand'] = ["fields(select=Name,Color,Quantity)"]

)
query_params = ItemsRequestBuilderGetQueryParameters()
query_params['expand'] = ["fields(select=Name,Color,Quantity)"]

)


result = await client.sites_by_id('site-id').lists_by_id('list-id').items.get(request_configuration)


```