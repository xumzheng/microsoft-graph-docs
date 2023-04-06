---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupRequestBuilderGetRequestConfiguration(
request_config = GroupRequestBuilderGetRequestConfiguration(query_params=query_params = GroupRequestBuilderGetQueryParameters()
query_params.select = ["*","parentSiteId"]

)
query_params = GroupRequestBuilderGetQueryParameters()
query_params.select = ["*","parentSiteId"]

)


result = await client.sites_by_id('site-id').termStore.groups_by_id('group-id').get(request_config, headers=request_config)


```