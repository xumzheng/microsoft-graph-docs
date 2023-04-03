---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = SchemaExtensionsRequestBuilderGetRequestConfiguration();

query_params = SchemaExtensionsRequestBuilderGetQueryParameters();
query_params.filter = "id eq 'graphlearn_test'";

request_config.queryParameters = query_params;


result = awaitclient.schemaExtensions().get(request_config);


```