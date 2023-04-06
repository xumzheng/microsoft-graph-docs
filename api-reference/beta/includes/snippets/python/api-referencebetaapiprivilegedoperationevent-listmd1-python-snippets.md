---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration(
request_configuration = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration(query_params=query_params = PrivilegedOperationEventsRequestBuilderGetQueryParameters()
query_params['filter'] = "requestType eq 'Activate'"

)
query_params = PrivilegedOperationEventsRequestBuilderGetQueryParameters()
query_params['filter'] = "requestType eq 'Activate'"

)


result = await client.privilegedOperationEvents.get(request_configuration)


```