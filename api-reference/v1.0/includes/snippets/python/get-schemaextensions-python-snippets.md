---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = SchemaExtensionsRequestBuilderGetRequestConfiguration(
query_params = SchemaExtensionsRequestBuilderGetQueryParameters()
query_params.filter = "id eq 'graphlearn_test'"

)


result = await client.schemaExtensions.get(request_config)


```