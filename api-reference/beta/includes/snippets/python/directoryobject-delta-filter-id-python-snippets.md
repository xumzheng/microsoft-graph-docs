---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = DeltaRequestBuilderGetRequestConfiguration();

query_params = DeltaRequestBuilderGetQueryParameters();
query_params.filter = "id eq '87d349ed-44d7-43e1-9a83-5f2406dee5bd'";

request_config.queryParameters = query_params;


result = awaitclient.directoryObjects().delta().get(request_config);


```