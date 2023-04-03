---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration();

query_params = PrivilegedOperationEventsRequestBuilderGetQueryParameters();
query_params.filter = "requestType eq 'Deactivate'";

request_config.queryParameters = query_params;


result = await client.privilegedOperationEvents().get(request_config);


```