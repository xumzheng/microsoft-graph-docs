---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = PrivilegedOperationEventsRequestBuilder.PrivilegedOperationEventsRequestBuilderGetQueryParameters(
		filter = "(creationDateTime ge 2017-06-25T07:00:00Z) and ",
		count = true,
		orderby = ["creationDateTime desc"],
)

request_configuration = PrivilegedOperationEventsRequestBuilder.PrivilegedOperationEventsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.privileged_operation_events.get(request_configuration = request_configuration)


```