---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = DeltaRequestBuilderGetRequestConfiguration();

query_params = DeltaRequestBuilderGetQueryParameters();
query_params.select = ["displayName","jobTitle","mail"];

headers = [
'Prefer' => 'return=minimal',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.contacts().delta().get(request_config);


```