---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ListItemRequestBuilderGetRequestConfiguration()

query_params = ListItemRequestBuilderGetQueryParameters()
query_params.expand = ["fields"]

request_config.queryParameters = query_params


result = await client.sites._by_id('site-id').lists._by_id('list-id').items._by_id('listItem-id').get(request_config)


```