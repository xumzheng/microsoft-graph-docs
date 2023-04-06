---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MembersRequestBuilderGetRequestConfiguration(
request_configuration = MembersRequestBuilderGetRequestConfiguration(query_params=query_params = MembersRequestBuilderGetQueryParameters()
query_params['count'] = true
query_params['filter'] = "startswith(displayName,%20'a')"

)
query_params = MembersRequestBuilderGetQueryParameters()
query_params['count'] = true
query_params['filter'] = "startswith(displayName,%20'a')"

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.groups_by_id('group-id').members.get(request_configuration)


```