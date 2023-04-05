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


result = await client.sitesby_id('site-id').listsby_id('list-id').itemsby_id('listItem-id').get(request_config)


```