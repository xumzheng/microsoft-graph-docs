---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = CloudPCRequestBuilderGetRequestConfiguration();

query_params = CloudPCRequestBuilderGetQueryParameters();
query_params.select = ["id","displayName","imageDisplayName","lastModifiedDateTime","lastRemoteActionResult","lastLoginResult","connectivityResult"];

request_config.queryParameters = query_params;


result = awaitclient.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').get(request_config);


```