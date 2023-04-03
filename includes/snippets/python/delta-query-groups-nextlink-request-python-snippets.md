---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = DeltaRequestBuilderGetRequestConfiguration();

query_params = DeltaRequestBuilderGetQueryParameters();
query_params.skiptoken = "pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvB7XnF_yllFsCrZJ";

request_config.queryParameters = query_params;


result = await client.groups().delta().get(request_config);


```