---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = AssignmentsRequestBuilderGetRequestConfiguration();

query_params = AssignmentsRequestBuilderGetQueryParameters();
query_params.expand = ["resources"];

request_config.queryParameters = query_params;


result = awaitclient.education().classesById('educationClass-id').assignments().get(request_config);


```