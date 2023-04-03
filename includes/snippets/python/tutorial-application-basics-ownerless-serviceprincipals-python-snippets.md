---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ServicePrincipalsRequestBuilderGetRequestConfiguration();

query_params = ServicePrincipalsRequestBuilderGetQueryParameters();
query_params.filter = "owners/$count eq 0 or owners/$count eq 1";
query_params.count = true;

headers = [
'ConsistencyLevel' => 'eventual',
];

request_config.queryParameters = query_params;
request_config.headers = headers;


result = awaitclient.servicePrincipals().get(request_config);


```