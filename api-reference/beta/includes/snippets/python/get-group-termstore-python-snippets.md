---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupRequestBuilderGetRequestConfiguration()

query_params = GroupRequestBuilderGetQueryParameters()
query_params.select = ["*","parentSiteId"]

request_config.queryParameters = query_params


result = await client.sites._by_id('site-id').termStore.groups._by_id('group-id').get(request_config)


```