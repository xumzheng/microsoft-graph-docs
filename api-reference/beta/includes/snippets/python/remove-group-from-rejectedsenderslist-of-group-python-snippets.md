---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RefRequestBuilderDeleteRequestConfiguration()

query_params = RefRequestBuilderDeleteQueryParameters()
query_params.id = "https://graph.microsoft.com/beta/groups/{other-group-id}"

request_config.queryParameters = query_params


await client.groupsby_id('group-id')_rejectedSenders_ref.delete(request_config)


```