---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ListItemRequestBuilderGetRequestConfiguration(
request_configuration = ListItemRequestBuilderGetRequestConfiguration(query_params=query_params = ListItemRequestBuilderGetQueryParameters()
query_params['expand'] = ["fields"]

)
query_params = ListItemRequestBuilderGetQueryParameters()
query_params['expand'] = ["fields"]

)


result = await client.sites_by_id('site-id').lists_by_id('list-id').items_by_id('listItem-id').get(request_configuration)


```