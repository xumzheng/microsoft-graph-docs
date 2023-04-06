---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RefRequestBuilderDeleteRequestConfiguration(
request_configuration = RefRequestBuilderDeleteRequestConfiguration(query_params=query_params = RefRequestBuilderDeleteQueryParameters()
query_params['id'] = "https://graph.microsoft.com/beta/users/{id}"

)
query_params = RefRequestBuilderDeleteQueryParameters()
query_params['id'] = "https://graph.microsoft.com/beta/users/{id}"

)


await client.groups_by_id('group-id').rejectedSenders.ref.delete(request_configuration)


```