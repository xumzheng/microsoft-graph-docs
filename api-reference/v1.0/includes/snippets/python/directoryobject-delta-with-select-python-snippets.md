---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeltaRequestBuilderGetRequestConfiguration()

query_params = DeltaRequestBuilderGetQueryParameters()
query_params.filter = "isof or isof"
query_params.select = ["microsoft.graph.user/surname","microsoft.graph.group/displayName"]

request_config.queryParameters = query_params


result = await client.directoryObjects.delta.get(request_config)


```