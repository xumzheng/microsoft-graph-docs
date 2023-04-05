---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration(
query_params = PrivilegedOperationEventsRequestBuilderGetQueryParameters()
query_params.filter = "(creationDateTime ge 2017-06-25T07:00:00Z) and "
query_params.count = true
query_params.orderby = ["creationDateTime desc"]

)


result = await client.privilegedOperationEvents.get(request_config)


```