---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration();

query_params = PrivilegedOperationEventsRequestBuilderGetQueryParameters();
query_params.filter = "(creationDateTime ge 2017-06-25T07:00:00Z) and ";
query_params.count = true;
query_params.orderby = ["creationDateTime desc"];

request_config.queryParameters = query_params;


result = awaitclient.privilegedOperationEvents().get(request_config);


```