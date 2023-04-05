---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = DeltaRequestBuilderGetRequestConfiguration()

query_params = DeltaRequestBuilderGetQueryParameters()
query_params.top = 3

request_config.queryParameters = query_params


result = await client.education.classes._by_id('educationClass-id').assignmentCategories.delta.get(request_config)


```