---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = MembersRequestBuilderGetRequestConfiguration()

query_params = MembersRequestBuilderGetQueryParameters()
query_params.filter = "roles/any"

request_config.queryParameters = query_params


result = await client.teamsById('team-id').members.get(request_config)


```