---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = DeltaRequestBuilder.DeltaRequestBuilderGetQueryParameters(
				filter = "isof or isof",
				select = ["microsoft.graph.user/surname","microsoft.graph.group/displayName"],
)

request_configuration = DeltaRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.directoryObjects.delta.get(request_configuration = request_configuration)


```