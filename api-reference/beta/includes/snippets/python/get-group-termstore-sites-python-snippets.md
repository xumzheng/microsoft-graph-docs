---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = GroupRequestBuilderGetRequestConfiguration(
)


result = await client.sites_by_id('site-id').termStore.groups_by_id('group-id').get()


```