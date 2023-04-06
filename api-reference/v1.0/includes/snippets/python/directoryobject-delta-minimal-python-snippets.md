---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = DeltaRequestBuilderGetRequestConfiguration(
request_configuration = DeltaRequestBuilderGetRequestConfiguration(query_params=query_params = DeltaRequestBuilderGetQueryParameters()
query_params['filter'] = "isof or isof"
query_params['select'] = ["microsoft.graph.user/surname","microsoft.graph.group/displayName"]

)
query_params = DeltaRequestBuilderGetQueryParameters()
query_params['filter'] = "isof or isof"
query_params['select'] = ["microsoft.graph.user/surname","microsoft.graph.group/displayName"]

System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.directoryObjects.delta.get(request_configuration)


```