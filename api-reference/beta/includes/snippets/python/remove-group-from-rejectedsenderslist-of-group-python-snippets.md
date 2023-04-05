---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RefRequestBuilderDeleteRequestConfiguration(
query_params = RefRequestBuilderDeleteQueryParameters()
query_params.id = "https://graph.microsoft.com/beta/groups/{other-group-id}"

)


await client.groups_by_id('group-id').rejectedSenders.ref.delete(request_config)


```