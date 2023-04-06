---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = GroupsRequestBuilderGetRequestConfiguration(
request_configuration = GroupsRequestBuilderGetRequestConfiguration(query_params=query_params = GroupsRequestBuilderGetQueryParameters()
query_params['filter'] = "createdDateTime ge 2021-11-01"
query_params['count'] = true

)
query_params = GroupsRequestBuilderGetQueryParameters()
query_params['filter'] = "createdDateTime ge 2021-11-01"
query_params['count'] = true

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.groups.get(request_configuration)


```