---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AttributeSetsRequestBuilder.AttributeSetsRequestBuilderGetQueryParameters(
				top = 10,
)

request_configuration = AttributeSetsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.directory.attributeSets.get(request_configuration = request_configuration)


```