---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ItemsRequestBuilder.ItemsRequestBuilderGetQueryParameters(
				expand = ["fields(select=Name,Color,Quantity)"],
)

request_configuration = ItemsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.sites_by_id('site-id').lists_by_id('list-id').items.get(request_configuration = request_configuration)


```