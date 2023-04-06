---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = SchemaExtensionsRequestBuilderGetRequestConfiguration(
request_configuration = SchemaExtensionsRequestBuilderGetRequestConfiguration(query_params=query_params = SchemaExtensionsRequestBuilderGetQueryParameters()
query_params['filter'] = "id eq 'graphlearn_test'"

)
query_params = SchemaExtensionsRequestBuilderGetQueryParameters()
query_params['filter'] = "id eq 'graphlearn_test'"

)


result = await client.schemaExtensions.get(request_configuration)


```