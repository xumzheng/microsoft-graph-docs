---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AttributeSetsRequestBuilderGetRequestConfiguration()

query_params = AttributeSetsRequestBuilderGetQueryParameters()
query_params.orderby = ["id"]

request_config.queryParameters = query_params


result = await client.directory_attributeSets.get(request_config)


```