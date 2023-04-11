---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = PrivilegedOperationEventsRequestBuilder.PrivilegedOperationEventsRequestBuilderGetQueryParameters(
				filter = "requestType eq 'Deactivate'",
)

request_configuration = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.privilegedOperationEvents.get(request_configuration = request_configuration)


```