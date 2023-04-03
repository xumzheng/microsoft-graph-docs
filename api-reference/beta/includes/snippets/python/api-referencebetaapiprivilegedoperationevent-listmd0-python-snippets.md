---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration();

query_params = PrivilegedOperationEventsRequestBuilderGetQueryParameters();
query_params.filter = "requestType eq 'Assign'";

request_config.queryParameters = query_params;


result = awaitclient.privilegedOperationEvents().get(request_config);


```