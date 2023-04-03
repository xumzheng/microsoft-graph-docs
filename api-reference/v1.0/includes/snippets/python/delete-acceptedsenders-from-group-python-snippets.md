---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = RefRequestBuilderDeleteRequestConfiguration();

query_params = RefRequestBuilderDeleteQueryParameters();
query_params.id = "https://graph.microsoft.com/v1.0/users/{user-id}";

request_config.queryParameters = query_params;


await client.groupsById('group-id').acceptedSenders().ref().delete(request_config);


```