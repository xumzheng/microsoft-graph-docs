---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeltaRequestBuilderGetRequestConfiguration(
request_config = DeltaRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "isof or isof"
params['select'] = ["microsoft.graph.user/surname","microsoft.graph.group/displayName"]
)


result = await client.directoryObjects.delta.get(request_config, headers=request_config)


```