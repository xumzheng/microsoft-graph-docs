---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = GroupRequestBuilderGetRequestConfiguration(
request_configuration = GroupRequestBuilderGetRequestConfiguration(query_params=query_params = GroupRequestBuilderGetQueryParameters()
query_params['count'] = true
query_params['orderby'] = ["displayName"]
query_params['filter'] = "startswith(displayName,%20'A')"

)
query_params = GroupRequestBuilderGetQueryParameters()
query_params['count'] = true
query_params['orderby'] = ["displayName"]
query_params['filter'] = "startswith(displayName,%20'A')"

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.devices_by_id('device-id').memberOf.graphgroup.get(request_configuration)


```