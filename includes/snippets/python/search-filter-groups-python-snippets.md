---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GroupsRequestBuilderGetRequestConfiguration(
request_config = GroupsRequestBuilderGetRequestConfiguration(query_params=query_params = GroupsRequestBuilderGetQueryParameters()
query_params.filter = "mailEnabled eq true"
query_params.search = "\"displayName:OneVideo\""

)
query_params = GroupsRequestBuilderGetQueryParameters()
query_params.filter = "mailEnabled eq true"
query_params.search = "\"displayName:OneVideo\""

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.groups.get(request_config, headers=request_config)


```