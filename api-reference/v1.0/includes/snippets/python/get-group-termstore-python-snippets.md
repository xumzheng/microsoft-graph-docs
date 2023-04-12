---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = GroupRequestBuilder.GroupRequestBuilderGetQueryParameters(
		select = ["*","parentSiteId"],
)

request_configuration = GroupRequestBuilder.GroupRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.sites_by_id('site-id').termStore.groups_by_id('group-id').get(request_configuration = request_configuration)


```