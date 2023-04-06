---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MembersRequestBuilderGetRequestConfiguration(
request_configuration = MembersRequestBuilderGetRequestConfiguration(query_params=query_params = MembersRequestBuilderGetQueryParameters()
query_params['filter'] = "roles/any"

)
query_params = MembersRequestBuilderGetQueryParameters()
query_params['filter'] = "roles/any"

)


result = await client.teams_by_id('team-id').members.get(request_configuration)


```