---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ListItemVersionRequestBuilder.ListItemVersionRequestBuilderGetQueryParameters(
		expand = ["fields"],
)

request_configuration = ListItemVersionRequestBuilder.ListItemVersionRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.sites_by_id('site-id').lists_by_id('list-id').items_by_id('listItem-id').versions_by_id('listItemVersion-id').get(request_configuration = request_configuration)


```